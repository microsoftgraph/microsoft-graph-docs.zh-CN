---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24d9d931ec6ffa44a1d840d45fae7eb6256ccd4e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993703"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.NamedLocationsRequestBuilderGetQueryParameters{
    Filter: "microsoft.graph.countryNamedLocation/countriesAndRegions/any(c:%20c%20eq%20'CA')",
}
options := &msgraphsdk.NamedLocationsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Identity().ConditionalAccess().NamedLocations().Get(options)


```