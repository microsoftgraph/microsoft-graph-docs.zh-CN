---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c50c33ff35669833ac333f3586c0d65f6a5ab304
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082617"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExtension()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.outlookServices.openTypeExtension",
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