# Steam Free License Remover

A tool to remove all Complimentary (free) package licenses from your Steam account.

## What it does

1. Logs into your Steam account
2. Fetches all your licenses and identifies complimentary (free) ones
3. Checks package info to verify they are FreeOnDemand and Available
4. Protects apps that are covered by paid licenses
5. Removes the free licenses after confirmation

## Protections

Apps are protected and will NOT be removed if:
- They are covered by a paid/non-complimentary license
- The package is no longer available (status != Available)
- The package billing type is not FreeOnDemand

## Output

- Console shows real-time progress of removals
- A log file `RemovedLicenses_{AccountID}.log` is created with all actions
- License list changes are tracked and displayed in real-time

## Disclaimer

**USE AT YOUR OWN RISK**

This tool is provided as-is with no warranty or support. If you remove something that:
- Wasn't actually free
- Cannot be obtained again
- Was a limited-time promotion

There is no support available. You are solely responsible for any licenses removed from your account.

## Usage

Install [.NET](https://dotnet.microsoft.com/download) and run:

```
dotnet run
```
