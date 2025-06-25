
## How to reach me 

TypeScript:
```ts 

async function get704Contact() {
  try {
    const res = await fetch("https://704consultancy.com/contact-me");
    const contact = await res.json();
    console.log("704's Contact Info:", contact);
  } catch (error) {
    console.error("Failed to fetch contact info:", error);
  }
}

```

Python:
```python 
from fastapi import FastAPI
import requests

app = FastAPI()

@app.get("/contact-me")
def fetch_contact():
    try:
        res = requests.get("https://704consultancy.com/contact-me")
        res.raise_for_status()
        return res.json()
    except requests.RequestException as e:
        return {"error": "Failed to fetch contact info", "details": str(e)}

```

cURL:
```console
curl https://704consultancy.com/contact-me | jq
```
