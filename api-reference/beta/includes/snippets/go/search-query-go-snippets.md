---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b5a2b078b73a96f36192b4d8ee51346132a8869
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031989"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetRequests( []SearchRequest {
    msgraphsdk.NewSearchRequest(),
    SetAdditionalData(map[string]interface{}{
        "entityTypes":  []String {
            "externalItem",
        }
        "contentSources":  []String {
            "/external/connections/connectionfriendlyname",
        }
        "from": ,
        "size": ,
        "fields":  []String {
            "title",
            "description",
        }
    }
}
options := &msgraphsdk.QueryRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Search().Query().Post(options)


```