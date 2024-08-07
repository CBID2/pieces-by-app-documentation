---
title: Tag API | TypeScript SDK
---

# Tag API

All URIs are relative to `http://localhost:1000`

Method | HTTP request | Description
------------- | ------------- | -------------
[**tagAssociateAsset**](TagApi#tagassociateasset) | **POST** /tag/\{tag\}/assets/associate/\{asset\} | /tag/\{tag\}/assets/associate/\{asset\} [POST]
[**tagAssociatePerson**](TagApi#tagassociateperson) | **POST** /tag/\{tag\}/persons/associate/\{person\} | /tag/\{tag\}/persons/associate/\{person\} [POST]
[**tagDisassociateAsset**](TagApi#tagdisassociateasset) | **POST** /tag/\{tag\}/assets/disassociate/\{asset\} | /tag/\{tag\}/assets/disassociate/\{asset\} [POST]
[**tagDisassociatePerson**](TagApi#tagdisassociateperson) | **POST** /tag/\{tag\}/persons/disassociate/\{person\} | /tag/\{tag\}/persons/disassociate/\{person\} [POST]
[**tagScoresIncrement**](TagApi#tagscoresincrement) | **POST** /tag/\{tag\}/scores/increment | \'/tag/\{tag\}/scores/increment\' [POST]
[**tagUpdate**](TagApi#tagupdate) | **POST** /tag/update | /tag/update [POST]
[**tagsSpecificTagSnapshot**](TagApi#tagsspecifictagsnapshot) | **GET** /tag/\{tag\} | /tag/\{tag\} [GET]


## **tagAssociateAsset** {#tagassociateasset}
> tagAssociateAsset()

This will associate a tag with a asset.

### Example {#tagassociateasset-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.TagApi(configuration)

const body: Pieces.TagAssociateAssetRequest = {
// string | The id (uuid) of the asset that you are trying to access.
asset: 2254f2c8-5797-40e8-ac56-41166dc0e159,
// string | tag id
tag: tag_example,
};

apiInstance.tagAssociateAsset(body).then((data: void (empty response body)) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#tagassociateasset-parameters}


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **asset** | [**string**] | The id (uuid) of the asset that you are trying to access. | defaults to undefined
 **tag** | [**string**] | tag id | defaults to undefined


### Return type {#tagassociateasset-return-type}

void (empty response body)

### HTTP request headers {#tagassociateasset-http-request-headers}

- **Content-Type**: Not defined
- **Accept**: text/plain


### HTTP response details {#tagassociateasset-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**204** | No Content |  -  |
**500** | Internal Server Error |  -  |

## **tagAssociatePerson** {#tagassociateperson}
> tagAssociatePerson()

This will associate a tag with a person.

### Example {#tagassociateperson-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.TagApi(configuration)

const body: Pieces.TagAssociatePersonRequest = {
// string | tag id
tag: tag_example,
// string | This is a uuid that represents a person.
person: person_example,
};

apiInstance.tagAssociatePerson(body).then((data: void (empty response body)) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#tagassociateperson-parameters}


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tag** | [**string**] | tag id | defaults to undefined
 **person** | [**string**] | This is a uuid that represents a person. | defaults to undefined


### Return type {#tagassociateperson-return-type}

void (empty response body)

### HTTP request headers {#tagassociateperson-http-request-headers}

- **Content-Type**: Not defined
- **Accept**: text/plain


### HTTP response details {#tagassociateperson-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**204** | No Content |  -  |
**500** | Internal Server Error |  -  |

## **tagDisassociateAsset** {#tagdisassociateasset}
> tagDisassociateAsset()

This will enable us to dissassociate a tag from a asset.

### Example {#tagdisassociateasset-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.TagApi(configuration)

const body: Pieces.TagDisassociateAssetRequest = {
// string | tag id
tag: tag_example,
// string | The id (uuid) of the asset that you are trying to access.
asset: 2254f2c8-5797-40e8-ac56-41166dc0e159,
};

apiInstance.tagDisassociateAsset(body).then((data: void (empty response body)) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#tagdisassociateasset-parameters}


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tag** | [**string**] | tag id | defaults to undefined
 **asset** | [**string**] | The id (uuid) of the asset that you are trying to access. | defaults to undefined


### Return type {#tagdisassociateasset-return-type}

void (empty response body)

### HTTP request headers {#tagdisassociateasset-http-request-headers}

- **Content-Type**: Not defined
- **Accept**: text/plain


### HTTP response details {#tagdisassociateasset-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**204** | No Content |  -  |
**500** | Internal Server Error |  -  |

## **tagDisassociatePerson** {#tagdisassociateperson}
> tagDisassociatePerson()

This will enable us to dissassociate a tag from a person.

### Example {#tagdisassociateperson-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.TagApi(configuration)

const body: Pieces.TagDisassociatePersonRequest = {
// string | tag id
tag: tag_example,
// string | This is a uuid that represents a person.
person: person_example,
};

apiInstance.tagDisassociatePerson(body).then((data: void (empty response body)) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#tagdisassociateperson-parameters}


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tag** | [**string**] | tag id | defaults to undefined
 **person** | [**string**] | This is a uuid that represents a person. | defaults to undefined


### Return type {#tagdisassociateperson-return-type}

void (empty response body)

### HTTP request headers {#tagdisassociateperson-http-request-headers}

- **Content-Type**: Not defined
- **Accept**: text/plain


### HTTP response details {#tagdisassociateperson-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**204** | No Content |  -  |
**500** | Internal Server Error |  -  |

## **tagScoresIncrement** {#tagscoresincrement}
> tagScoresIncrement()

This will take in a SeededScoreIncrement and will increment the material relative to the incoming body.

### Example {#tagscoresincrement-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.TagApi(configuration)

const body: Pieces.TagScoresIncrementRequest = {
// string | tag id
tag: tag_example,
// SeededScoreIncrement (optional)
seededScoreIncrement: ,
};

apiInstance.tagScoresIncrement(body).then((data: void (empty response body)) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#tagscoresincrement-parameters}


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **seededScoreIncrement** | **SeededScoreIncrement**|  |
 **tag** | [**string**] | tag id | defaults to undefined


### Return type {#tagscoresincrement-return-type}

void (empty response body)

### HTTP request headers {#tagscoresincrement-http-request-headers}

- **Content-Type**: application/json
- **Accept**: text/plain


### HTTP response details {#tagscoresincrement-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**204** | No Content |  -  |
**500** | Internal Server Error |  -  |

## **tagUpdate** {#tagupdate}
> Tag tagUpdate()

This will update a specific tag.

### Example {#tagupdate-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.TagApi(configuration)

const body: Pieces.TagUpdateRequest = {
// boolean | This is a boolean that will decided if we are want to return the transferable data (default) or not(performance enhancement) (optional)
transferables: true,
// Tag (optional)
tag: ,
};

apiInstance.tagUpdate(body).then((data: Tag) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#tagupdate-parameters}


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tag** | **Tag**|  |
 **transferables** | [**boolean**] | This is a boolean that will decided if we are want to return the transferable data (default) or not(performance enhancement) | (optional) defaults to undefined


### Return type {#tagupdate-return-type}

[**Tag**](../models/Tag)

### HTTP request headers {#tagupdate-http-request-headers}

- **Content-Type**: application/json
- **Accept**: application/json, text/plain


### HTTP response details {#tagupdate-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**200** | OK |  -  |
**500** | Internal Server Error |  -  |

## **tagsSpecificTagSnapshot** {#tagsspecifictagsnapshot}
> Tag tagsSpecificTagSnapshot()

This will get a specific tag.

### Example {#tagsspecifictagsnapshot-example}

```typescript
import * as Pieces from '@pieces.app/pieces-os-client'

const configuration = Pieces.Configuration()
const apiInstance = new Pieces.TagApi(configuration)

const body: Pieces.TagsSpecificTagSnapshotRequest = {
// string | tag id
tag: tag_example,
// boolean | This is a boolean that will decided if we are want to return the transferable data (default) or not(performance enhancement) (optional)
transferables: true,
};

apiInstance.tagsSpecificTagSnapshot(body).then((data: Tag) => {
console.log('API called successfully. Returned data: ' + data)
}).catch((error: unknown) => console.error(error))
```

### Parameters {#tagsspecifictagsnapshot-parameters}


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tag** | [**string**] | tag id | defaults to undefined
 **transferables** | [**boolean**] | This is a boolean that will decided if we are want to return the transferable data (default) or not(performance enhancement) | (optional) defaults to undefined


### Return type {#tagsspecifictagsnapshot-return-type}

[**Tag**](../models/Tag)

### HTTP request headers {#tagsspecifictagsnapshot-http-request-headers}

- **Content-Type**: Not defined
- **Accept**: application/json, text/plain


### HTTP response details {#tagsspecifictagsnapshot-http-response-details}
| Status code | Description | Response headers
|-------------|-------------|------------------
**200** | OK |  -  |
**410** | Tag was not found. |  -  |


