# IP4 to Binary Converter

This Bash script allows you to convert an IPV4 address from decimal format to binary format. You can use it to obtain the binary representation of an IP address.

## Usage

./ip4tobin [OPTIONS] IP_ADDRESS

### Arguments

- `IP_ADDRESS`: The IP address to convert in decimal format.

### Options

- `-h, --help`: Display the help message with usage information for the script.
- `-nd, --nodot`: Do not display dots between octets in the binary output.
- `-d, --details`: Show detailed output with headers for each octet.

## Usage Examples

1. Convert a decimal IP address to binary:
./ip4tobin 192.168.1.1

2. Convert an IP address without dots between octets:
./ip4tobin -nd 19216811

3. Show the output in detailed format:
./ip4tobin -d 192.168.1.1

4. Display the help message:
./ip4tobin -h

## Error Handling

- If the `bc` command is not available on your system, an error message will be displayed.
- If you do not have execution permissions for the script, an error message will be shown.
- If the IP argument is missing, an error message with usage instructions will be displayed.

## Error Examples

- Example of an error when 'bc' is not available:

Error: The 'bc' command is not available on this system. Please install it or check your PATH environment variable.


- Example of an error when execution permissions are missing:

Error: Insufficient permissions to execute this script. Please ensure the script is executable.


- Example of an error when the IP argument is missing:

Error: IP address argument is missing. Usage: ./ip4tobin [OPTIONS] IP_ADDRESS

## Requirements

Ensure that you have the `bc` command installed on your system, as the script uses it for mathematical operations.

## Author

Daniele Franceschini