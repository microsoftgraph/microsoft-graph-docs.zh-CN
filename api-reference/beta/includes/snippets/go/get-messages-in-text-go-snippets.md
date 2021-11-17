---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc71fa3d3c7a734570fa88b817e4845c594f17ad
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033383"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.MessagesRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,uniqueBody",
}
headers := map[string]string{
    "Prefer": "outlook.body-content-type="text""
}
options := &msgraphsdk.MessagesRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
result, err := graphClient.Me().Messages().Get(options)


```