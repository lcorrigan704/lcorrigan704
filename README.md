
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
import requests

def get_contact_info():
    url = "https://704consultancy.com/contact-me"
    response = requests.get(url)
    response.raise_for_status()  

    contact = response.json()
    print("704's Contact Info:")
    print(f"Email: {contact['email_address']}")
    print(f"Phone: {contact['phone_number']}")
    print(f"Message: {contact['message']}")

if __name__ == "__main__":
    get_contact_info()


```

cURL:
```console
curl https://704consultancy.com/contact-me | jq
```
