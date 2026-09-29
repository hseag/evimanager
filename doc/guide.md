# User Guide

## Prerequisites

- Windows
- A supported instrument: `eviDense UV` Photometer or `eviFluor Duo` Fluorometer
- A USB-C cable to connect the instrument to the computer
- Administrator rights, if you use the installer

## Install or run eviManager

Run the downloaded portable EXE directly. No installation is required; it extracts its bundled runtime and configuration on first use.

See [Downloads](downloads.md).

## Connect an instrument

Start eviManager and connect the `eviDense UV` or `eviFluor Duo` to the computer using the USB-C cable. While no instrument is connected, eviManager shows a placeholder screen; once an instrument is detected, the corresponding screen appears automatically.

## Information

The **Information** tab shows the connected instrument's type and model, its serial number, and its current firmware version.

## Firmware update

Open the **Firmware update** tab, which shows the currently installed firmware version.

1. Click **Browse...** and select the new firmware image (a `.srec` file).
2. Click **Start update** and wait for the update to complete.

Do not disconnect the instrument while an update is running.

## Instrument self-test

Open the **Instrument self-test** tab.

1. Click **Start test** to run the self-test.
2. Review the **Status**, **Date/Time**, and **Test result** fields once the test finishes.
3. Click **Export...** to save the test result as a PDF report.

## Basic functionalities

The **Basic functionalities** tab lets you set the instrument's status LED for service checks: **Red**, **Green**, **Blue** (and **White** on `eviFluor Duo`).
