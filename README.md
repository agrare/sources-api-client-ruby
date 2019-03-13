# sources-api-client

SourcesApiClient - the Ruby gem for the Sources

Sources

This SDK is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 0.1.0
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.RubyClientCodegen

## Installation

### Build a gem

To build the Ruby code into a gem:

```shell
gem build sources-api-client.gemspec
```

Then either install the gem locally:

```shell
gem install ./sources-api-client-1.0.0.gem
```
(for development, run `gem install --dev ./sources-api-client-1.0.0.gem` to install the development dependencies)

or publish the gem to a gem hosting service, e.g. [RubyGems](https://rubygems.org/).

Finally add this to the Gemfile:

    gem 'sources-api-client', '~> 1.0.0'

### Install from Git

If the Ruby gem is hosted at a git repository: https://github.com/GIT_USER_ID/GIT_REPO_ID, then add the following in the Gemfile:

    gem 'sources-api-client', :git => 'https://github.com/GIT_USER_ID/GIT_REPO_ID.git'

### Include the Ruby code directly

Include the Ruby code directly using `-I` as follows:

```shell
ruby -Ilib script.rb
```

## Getting Started

Please follow the [installation](#installation) procedure and then run the following code:
```ruby
# Load the gem
require 'sources-api-client'

# Setup authorization
SourcesApiClient.configure do |config|
  # Configure HTTP basic authorization: UserSecurity
  config.username = 'YOUR USERNAME'
  config.password = 'YOUR PASSWORD'
end

api_instance = SourcesApiClient::DefaultApi.new
authentication = SourcesApiClient::Authentication.new # Authentication | Authentication attributes to create

begin
  #Create a new Authentication
  result = api_instance.create_authentication(authentication)
  p result
rescue SourcesApiClient::ApiError => e
  puts "Exception when calling DefaultApi->create_authentication: #{e}"
end

```

## Documentation for API Endpoints

All URIs are relative to *https://virtserver.swaggerhub.com/r/insights/platform/sources/v0.1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*SourcesApiClient::DefaultApi* | [**create_authentication**](docs/DefaultApi.md#create_authentication) | **POST** /authentications | Create a new Authentication
*SourcesApiClient::DefaultApi* | [**create_endpoint**](docs/DefaultApi.md#create_endpoint) | **POST** /endpoints | Create a new Endpoint
*SourcesApiClient::DefaultApi* | [**create_source**](docs/DefaultApi.md#create_source) | **POST** /sources | Create a new Source
*SourcesApiClient::DefaultApi* | [**create_source_type**](docs/DefaultApi.md#create_source_type) | **POST** /source_types | Create a new SourceType
*SourcesApiClient::DefaultApi* | [**delete_authentication**](docs/DefaultApi.md#delete_authentication) | **DELETE** /authentications/{id} | Delete an existing Authentication
*SourcesApiClient::DefaultApi* | [**delete_endpoint**](docs/DefaultApi.md#delete_endpoint) | **DELETE** /endpoints/{id} | Delete an existing Endpoint
*SourcesApiClient::DefaultApi* | [**delete_source**](docs/DefaultApi.md#delete_source) | **DELETE** /sources/{id} | Delete an existing Source
*SourcesApiClient::DefaultApi* | [**get_documentation**](docs/DefaultApi.md#get_documentation) | **GET** /openapi.json | Return this API document in JSON format
*SourcesApiClient::DefaultApi* | [**list_authentications**](docs/DefaultApi.md#list_authentications) | **GET** /authentications | List Authentications
*SourcesApiClient::DefaultApi* | [**list_endpoint_authentications**](docs/DefaultApi.md#list_endpoint_authentications) | **GET** /endpoints/{id}/authentications | List Authentications for Endpoint
*SourcesApiClient::DefaultApi* | [**list_endpoints**](docs/DefaultApi.md#list_endpoints) | **GET** /endpoints | List Endpoints
*SourcesApiClient::DefaultApi* | [**list_source_availabilities**](docs/DefaultApi.md#list_source_availabilities) | **GET** /sources/{id}/availabilities | List Availabilities for Source
*SourcesApiClient::DefaultApi* | [**list_source_endpoints**](docs/DefaultApi.md#list_source_endpoints) | **GET** /sources/{id}/endpoints | List Endpoints for Source
*SourcesApiClient::DefaultApi* | [**list_source_type_availabilities**](docs/DefaultApi.md#list_source_type_availabilities) | **GET** /source_types/{id}/availabilities | List Availabilities for SourceType
*SourcesApiClient::DefaultApi* | [**list_source_type_sources**](docs/DefaultApi.md#list_source_type_sources) | **GET** /source_types/{id}/sources | List Sources for SourceType
*SourcesApiClient::DefaultApi* | [**list_source_types**](docs/DefaultApi.md#list_source_types) | **GET** /source_types | List SourceTypes
*SourcesApiClient::DefaultApi* | [**list_sources**](docs/DefaultApi.md#list_sources) | **GET** /sources | List Sources
*SourcesApiClient::DefaultApi* | [**show_authentication**](docs/DefaultApi.md#show_authentication) | **GET** /authentications/{id} | Show an existing Authentication
*SourcesApiClient::DefaultApi* | [**show_endpoint**](docs/DefaultApi.md#show_endpoint) | **GET** /endpoints/{id} | Show an existing Endpoint
*SourcesApiClient::DefaultApi* | [**show_source**](docs/DefaultApi.md#show_source) | **GET** /sources/{id} | Show an existing Source
*SourcesApiClient::DefaultApi* | [**show_source_type**](docs/DefaultApi.md#show_source_type) | **GET** /source_types/{id} | Show an existing SourceType
*SourcesApiClient::DefaultApi* | [**update_authentication**](docs/DefaultApi.md#update_authentication) | **PATCH** /authentications/{id} | Update an existing Authentication
*SourcesApiClient::DefaultApi* | [**update_endpoint**](docs/DefaultApi.md#update_endpoint) | **PATCH** /endpoints/{id} | Update an existing Endpoint
*SourcesApiClient::DefaultApi* | [**update_source**](docs/DefaultApi.md#update_source) | **PATCH** /sources/{id} | Update an existing Source


## Documentation for Models

 - [SourcesApiClient::Authentication](docs/Authentication.md)
 - [SourcesApiClient::AuthenticationsCollection](docs/AuthenticationsCollection.md)
 - [SourcesApiClient::AvailabilitiesCollection](docs/AvailabilitiesCollection.md)
 - [SourcesApiClient::Availability](docs/Availability.md)
 - [SourcesApiClient::CollectionLinks](docs/CollectionLinks.md)
 - [SourcesApiClient::CollectionMetadata](docs/CollectionMetadata.md)
 - [SourcesApiClient::Endpoint](docs/Endpoint.md)
 - [SourcesApiClient::EndpointsCollection](docs/EndpointsCollection.md)
 - [SourcesApiClient::OrderParameters](docs/OrderParameters.md)
 - [SourcesApiClient::Source](docs/Source.md)
 - [SourcesApiClient::SourceType](docs/SourceType.md)
 - [SourcesApiClient::SourceTypesCollection](docs/SourceTypesCollection.md)
 - [SourcesApiClient::SourcesCollection](docs/SourcesCollection.md)
 - [SourcesApiClient::Tagging](docs/Tagging.md)


## Documentation for Authorization


### UserSecurity

- **Type**: HTTP basic authentication
