# Web stack

### Quick start

# Issue 1

## how to reproduce

```
openstack stack create -t stack.yaml stack --wait
openstack stack output show stack --all
```

### Results

```
+-----------+-------------------------------------------------------------------------------------------+
| Field     | Value                                                                                     |
+-----------+-------------------------------------------------------------------------------------------+
| server_ip | {                                                                                         |
|           |   "output_value": null,                                                                   |
|           |   "output_error": "The Referenced Attribute (host1 server.first_address) is incorrect.",  |
|           |   "output_key": "server_ip",                                                              |
|           |   "description": "server ip"                                                              |
|           | }                                                                                         |
+-----------+-------------------------------------------------------------------------------------------+
```

### Expected:

Should show the ip address of the instance from the nested resource
