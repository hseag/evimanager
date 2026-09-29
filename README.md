# eviManager

eviManager is a Windows service application for supported HSE AG Colibri
instruments. It gives service personnel one place to identify an instrument,
inspect its status and perform routine maintenance tasks.

## What eviManager does

When a supported instrument is connected by USB, eviManager detects it and
shows its model, serial number and installed firmware version. Depending on the
instrument, the application can:

- update firmware from an approved `.srec` firmware image;
- run the instrument self-test;
- export the self-test result as a PDF technical report; and
- control the instrument status LED during service checks.

eviManager supports the `eviDense UV` photometer and the `eviFluor Duo`
fluorometer.

## Who it is for

eviManager is intended for trained service personnel maintaining supported
Colibri instruments. It is not an instrument control application for routine
measurements. Use only firmware supplied for the connected instrument and do
not disconnect the USB cable while a firmware update is in progress.

## Getting started

Download the current Windows x64 portable executable from
[`downloads/`](downloads/). The download includes the required .NET runtime
and can be run directly; no separate installation is necessary. Connect the
instrument with a USB-C cable and start eviManager. The application selects the
appropriate interface after it detects the instrument.

For detailed instructions, see the [User Guide](doc/guide.md). The matching
SHA-256 checksum is published alongside each download.
