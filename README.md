# Device Registry Service

## Usage

All responses will have the form.



```json
{
  "data":"Mixed type of holding the content of the response",
  "message":"Description of what happened"
}
```

subsequent response definition will only detail the expected value of the `data field`

### List all devices

**Definition**

`GET /devices`

**Response**

- `200 OK` on success

```json

[
  {
    "identifier": "floor-lamp",
    "name":"Floor Lamp"
    "device_type":"switch",
    "controller_gateway":"192.168.0.2"
    
    },
    {
      "identifier": "samsung-tv",
      "name":"Living room TV"
      "device_type":"tv",
      "controller_gateway":"192.168.0.9"
    }
 ]
 
 ### Registering a new device 
 
 **Definition**
 
 `POST /devices`
 
 **Argumnets**
 
 
    
