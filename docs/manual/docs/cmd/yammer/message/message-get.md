# yammer message get

Returns a Yammer message

## Usage

```sh
yammer message get [options]
```

## Options

Option|Description
------|-----------
`--help`|output usage information
`--id <id>`|The id of the Yammer message
`--query [query]`|JMESPath query string. See [http://jmespath.org/](http://jmespath.org/) for more information and examples
`-o, --output [output]`|Output type. `json,text`. Default `text`
`--pretty`|Prettifies `json` output
`--verbose`|Runs command with verbose logging
`--debug`|Runs command with debug logging

## Remarks

!!! attention
    In order to use this command, you need to grant the Azure AD application used by the Office 365 CLI the permission to the Yammer API. To do this, execute the `consent --service yammer` command.

## Examples

Returns the Yammer message with the id 1239871123

```sh
yammer message get --id 1239871123
```

Returns the Yammer message with the id 1239871123 in JSON format

```sh
yammer message get --id 1239871123 --output json
```
