# terraform-hashicups-provider
# Overall architecture
[terraform core] <--RPC--> [resources, data sources and provider] <--Go--> [client library] <--HTTPs--> [target API]
# Why create a provider 
1. update existing provider 
- contribute bug fixes and updates 
- some providers may use SDKv2 (older framework)
2. create and publish a new provider 
3. create a custom provider 
- manage internal apps with Terraform 
- use private registry to distribute internally 
# Lab scenario 
- perform `plan, apply and destroy` against a fictional `Hashicups API`
- files 
    - main.go 
    - provider.go 
    - provider_test.go 
    - resource_order.go 
    - resource_order_test.go 
    - data_source.go 
    - data_source_test.go 
# New framework 
- better data type handling 
- allow writing custom data types 
- logging, tests, and generating docs etc 
## Prerequisites 
1. API, client library 
2. Provider framework 
- via terraform plugin framework
3. provider scaffolding 
- template to being creating provider 
- includes examples and boilerplate files 
- via a sample github repo 
# Lab scenario 
- setup development environment 
- configure hashicups client 
- implement data source 
- implement logging 
- implement resource create and read 

