---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca028019f23a51fc06efe8e08ea76c8a223f1912
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412580"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewRequestsRequestBody()
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