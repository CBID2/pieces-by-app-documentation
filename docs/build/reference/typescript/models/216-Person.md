---
title: Person | TypeScript SDK
---


# Person

if expiration is add then, after the alloted expiration date the user will only have view && comment only permissions. Only present in the case there is a scope such as a defined collection/asset...  if asset is passed then that means this person belongs to a scoped asset.  NOTE****: annotations here are annotations to describe the person!!! if in the future we want to add who wrote an annotation on and asset or soemthing like that, we will want to add a new field on here called authorships.

## Properties

Name | Type
------------ | -------------
**schema** | [**EmbeddedModelSchema**](EmbeddedModelSchema)
**id** | **string**
**created** | [**GroupedTimestamp**](GroupedTimestamp)
**updated** | [**GroupedTimestamp**](GroupedTimestamp)
**deleted** | [**GroupedTimestamp**](GroupedTimestamp)
**type** | [**PersonType**](PersonType)
**assets** | [**FlattenedAssets**](FlattenedAssets)
**mechanisms** | [**\{ [key: string]: MechanismEnum; \}**](MechanismEnum)
**interactions** | **number**
**access** | [**\{ [key: string]: PersonAccess; \}**](PersonAccess)
**tags** | [**FlattenedTags**](FlattenedTags)
**websites** | [**FlattenedWebsites**](FlattenedWebsites)
**models** | [**\{ [key: string]: PersonModel; \}**](PersonModel)
**annotations** | [**FlattenedAnnotations**](FlattenedAnnotations)
**score** | [**Score**](Score)
**summaries** | [**FlattenedWorkstreamSummaries**](FlattenedWorkstreamSummaries)

## Example

```typescript
import { Person } from '@pieces.app/pieces-os-client'

// TODO: Update the object below with actual values
const example: Person = {
    "schema": null,
    "id": null,
    "created": null,
    "updated": null,
    "deleted": null,
    "type": null,
    "assets": null,
    "mechanisms": null,
    "interactions": null,
    "access": null,
    "tags": null,
    "websites": null,
    "models": null,
    "annotations": null,
    "score": null,
    "summaries": null,
}

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Person
console.log(exampleParsed)
```

