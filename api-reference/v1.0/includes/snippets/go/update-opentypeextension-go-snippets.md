---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69f977d5d8d6f31e170ce654f1077189ac85e218
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003826"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewExtension()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2016-07-30T11:00:00.000Z",
    "DealValue": ,
    "topPicks":  []String {
        "Employees only",
        "Add spouse or guest",
        "Add family",
    }
}
options := &msgraphsdk.ExtensionRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
postId := "post-id"
extensionId := "extension-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).PostsById(&postId).ExtensionsById(&extensionId).Patch(options)


```