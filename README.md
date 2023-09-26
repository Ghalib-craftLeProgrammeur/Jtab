# jtab - JSON Table Formatter From Wlezz

`jtab` is a command-line tool written in Go for formatting JSON data as tables. It reads JSON data from a file and presents it in a tabular format. This tool is especially useful for visualizing structured JSON data in the terminal.

## Usage

### Prerequisites

Before using `jtab`, make sure you have Go installed on your system.

### Installation

Clone this repository and build the executable:

```bash
git clone https://github.com/yourusername/jtab.git

cd jtab
go build jtab.go
```
Usage
To use jtab, provide a JSON file as a command-line argument:

```bash
jtab.exe <JSON file>
```
Replace <JSON file> with the path to your JSON file.

### Features
Reads JSON data from a file.
Formats the data as a table.
Supports displaying structured data in a more readable way.
Example
Assuming you have a JSON file named data.json with the following content:

```json

[
  {
    "name": "John",
    "age": 30,
    "city": "New York"
  },
  {
    "name": "Alice",
    "age": 25,
    "city": "San Francisco"
  }
]
```
You can format it as a table like this:

```bash
./jtab data.json
```
This will display the JSON data in a tabular format:

```sql

┌─────┬─────┬────────────────┐
│ age │ city│ name           │
├─────┼─────┼────────────────┤
│ 30  │ New York   │ John   │
│ 25  │ San Francisco  │ Alice  │
└─────┴─────┴────────────────┘
```
### Customization
You can customize the jtab tool to fit your needs. For example, you can modify the table style using the SetStyle method or add more formatting options.

Dependencies
go-pretty(https://pkg.go.dev/github.com/jedib0t/go-pretty/v6/table) - A library for rendering and formatting tables in the terminal.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
Thanks to the go-pretty library for providing the table rendering functionality.
Feel free to contribute to this project or use it as a template for your own Go command-line tools!
