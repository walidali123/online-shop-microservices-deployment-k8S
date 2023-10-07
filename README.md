# online-shop-microservices-deployment-k8S
# online-shop-microservices-deployment
# Project README

This README provides an overview of the project code and its associated releases. The project manages a collection of microservices using Helm charts and provides configuration values for each service. 

## Releases

### rediscart
- **Chart**: `charts/redis`
- **Values**: 
  - `values/redis-values.yaml`
  - `appReplicas: "1"`
  - `volumeName: "redis-cart-data"`

### emailservice
- **Chart**: `charts/microservice`
- **Values**: 
  - `values/email-service-values.yaml`

### cartservice
- **Chart**: `charts/microservice`
- **Values**: 
  - `values/cart-service-values.yaml`

### currencyservice
- **Chart**: `charts/microservice`
- **Values**: 
  - `values/currency-service-values.yaml`

### paymentservice
- **Chart**: `charts/microservice`
- **Values**: 
  - `values/payment-service-values.yaml`

### recommendationservice
- **Chart**: `charts/microservice`
- **Values**: 
  - `values/recommendation-service-values.yaml`

### productcatalogservice
- **Chart**: `charts/microservice`
- **Values**: 
  - `values/productcatalog-service-values.yaml`

### shippingservice
- **Chart**: `charts/microservice`
- **Values**: 
  - `values/shipping-service-values.yaml`

### adservice
- **Chart**: `charts/microservice`
- **Values**: 
  - `values/ad-service-values.yaml`

### checkoutservice
- **Chart**: `charts/microservice`
- **Values**: 
  - `values/checkout-service-values.yaml`

### frontendservice
- **Chart**: `charts/microservice`
- **Values**: 
  - `values/frontend-values.yaml`

## Project Description

This project is a collection of microservices, each managed as a separate Helm release. The releases are organized by service name, with each service having its Helm chart and associated configuration values.

To deploy these microservices, you can use Helm to install each release separately, providing the corresponding chart and values file. Make sure to customize the values as needed for your specific deployment.

For example, to deploy the `rediscart` service, you can use the following Helm command:

```bash
helm install rediscart charts/redis -f values/redis-values.yaml --set appReplicas="1" --set volumeName="redis-cart-data"
```

Repeat this process for each of the other services, replacing the release name, chart, and values file as necessary.

Feel free to refer to the documentation of each microservice's Helm chart and values file for further customization options and deployment instructions.

**Note**: Ensure that you have Helm installed and configured in your environment before deploying these microservices.

## License

This project is distributed under the XYZ License. See the [LICENSE](LICENSE) file for details.

## Contact Information

For any questions or issues related to this project, please contact the project maintainers:

- [Maintainer Name](mailto:maintainer@example.com)

Thank you for using our project!
