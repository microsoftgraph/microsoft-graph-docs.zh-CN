---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6d18d5c5ace3aef4b31db52c3b237deffb5115c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101366"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.NamedLocationsRequestBuilderGetQueryParameters{
    Filter: "microsoft.graph.countryNamedLocation/countriesAndRegions/any(c:%20c%20eq%20'CA')",
}
options := &msgraphsdk.NamedLocationsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Identity().ConditionalAccess().NamedLocations().Get(options)


```