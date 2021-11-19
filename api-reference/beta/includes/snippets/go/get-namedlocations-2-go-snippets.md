---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23b546d2b7bd54d53712cd41a9e45208250a4c56
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094111"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.NamedLocationsRequestBuilderGetQueryParameters{
    Filter: "isof('microsoft.graph.ipNamedLocation')",
}
options := &msgraphsdk.NamedLocationsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Identity().ConditionalAccess().NamedLocations().Get(options)


```