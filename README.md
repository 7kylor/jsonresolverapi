 
## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.
 
Put your open ai key in: src/app/lib/openai.ts



# JSON Resolver API
This is a Next.js project that provides an API endpoint for converting unstructured data into a specified JSON format.

# API Usage
The API endpoint is a POST request that accepts a JSON body with two properties: data and format.

data is a string of unstructured data.

format is an object that describes the desired output JSON structure.

Here is an example of how to use the API with Postman:
 
POST http://localhost:3000/api/json

 {
    "data": "the test is name ahmed",
    "format": {
        "name": {
            "type": "number"
        }
    }
}

In this example, the data is "the test is name ahmed", and the format specifies that the output JSON should have a name property of type number.

The API will attempt to parse the data and convert it into the specified format. If successful, it will return a JSON response with the parsed data. If it encounters an error, it will return an error message.
