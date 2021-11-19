---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77ec869733f1028750a8f6431cf3b2d212db589a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086791"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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