# Android SDK Role

Installs Android SDK and updates different components depending on the
specified installation type.

## Role Variables

Depending on which kind of installation do you require, you can set the
variable ``android_sdk_mode`` to the following values:

* ``basic`` - Installs basic SDK files without additional tools.
* ``compiler`` - Installs compiler SDK components and tools.
* ``emulator`` - Installs emulator SDK system images.

## Dependencies

- pablerass.oracle-jvm

## Example Playbooks

### Basic Android SDK:

    - { role: android-sdk }

### Emulator:

    - { role: android-sdk, android_sdk_mode: emulator }

### Compiler:

    - { role: android-sdk, android_sdk_mode: compiler }

## Licenste

LGPLv3
