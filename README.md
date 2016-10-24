# Apigee-4MV4D-RaiseFaultPolicy-CustomFaults
An API Proxy bundle that demonstrates the RaiseFaultPolicy - Custom Faults
## Example

Consider a scenario where you need to validate some business logic & raise a custom fault if validation fails. Implementing same in target server will be sometime time consuming process due to various reasons like complex server architecture, legacy system logic, complex lifecycle process.

Let's say you would like to send back 400 bad request error response to the client & raise a custom fault when validation fails. It's very simple to implement same in Apigee Edge by creating a proxy & using RaiseFaultPolicy.

Above example proxy demonstrates how to restrict query params to target server & raise a fault if any query params present. You can modify the condition to suit your requirements using the flow variables.

For example,

API Request 1 - GET /hello - 200 OK

API Request 2 - GET /hello?name=Apigee - 400 BAD REQUEST


## How to use above bundle ?

1. Download zip file from /bundle/apiproxy.zip
2. Create a new proxy in Apigee Edge
3. Choose 'Proxy Bundle' option in Build a proxy screen
4. Upload apiproxy.zip
5. Once proxy is created, Deploy same to environment.
6. Make API calls to see policy in action.

## 4MV4D Video Link

[Apigee-4MV4D-RaiseFaultPolicy-CustomFaults-Demo](https://www.youtube.com/watch?v=zeH22r_6xXw)
