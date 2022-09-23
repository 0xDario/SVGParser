# Compile C from source and Installation of Node App Instructions

## 1. Install dependencies

```Bash
sudo apt-get install libxml2-dev make gcc nodejs npm
```

## 2. Compile Shared Library

From the root of the parser/ directory

```Bash
make
```

## 3. Install

From the root of the SVGApp/ directory

```Bash
npm install
```

## 4. Running Server

PORT is your personally given port number, e.g. 3000

Server will be accessible at `http://localhost:PORT`

```Bash
npm run dev PORT
```

## Directory Structure

```Bash
# This contains the Backend Node Server, with our Web Application and API
app.js

# These are the package configuration files for npm to install dependencies
package.json
package-lock.json

# This is the Frontend HTML file that you see when you visit the document root
public/index.html

# This is the Frontend browser JavaScript file
public/index.js

# This is the Frontend Custom Style Sheet file
public/style.css

# This is the directory for uploaded .svg files
upload/

# This is the directory where you put all your C parser code
parser/

```

Note: tested on Node.js ver.12.13.0
