

# veve-nft-bot
This is a tool to automatically click on the Veve app at the exact moment an NFT drop happens. It can be used with multiple phones simultaneously.

## Installation:
Download the latest release.
## Usage:

Connect your phone(s) to your computer. Make sure USB debugging is enabled on your phone(s).
Open the Veve app on your phone(s) and navigate to the NFT drop screen.
Run the executable file from your computer's terminal or command prompt, providing the necessary arguments.
The syntax to run the executable is:

`./veve-nft-bot --time DROP_TIME --get_x GET_X --get_y GET_Y --buy_x BUY_X --buy_y BUY_Y --device DEVICE_ID`

Replace each argument with the appropriate value:

- `DROP_TIME`: The time of the NFT drop in HH:MM:SS format. This is when the first click will occur.
- `GET_X` and `GET_Y`: The x and y coordinates (in pixels) of the initial click location on your phone's screen.
- `BUY_X` and `BUY_Y`: The x and y coordinates (in pixels) of the buy button location on your phone's screen.
- `DEVICE_ID`: The ID of the device you want to use. This is optional. If not provided, the program will use the first available device.

## Example:

`./veve-nft-bot --time 12:30:00 --get_x 100 --get_y 200 --buy_x 300 --buy_y 400 --device emulator-5554`

If you want to use the tool with multiple phones, repeat step 3 for each phone, providing the unique device ID for each one.

## Important Notes:

Make sure the Veve app is open and on the NFT drop screen at the time you specify for the drop.
The device ID can be found by running 'adb devices' in your terminal or command prompt.
The x and y coordinates should be determined based on your phone's screen resolution. They specify where the "Get" and "Buy" buttons are located on the screen.
