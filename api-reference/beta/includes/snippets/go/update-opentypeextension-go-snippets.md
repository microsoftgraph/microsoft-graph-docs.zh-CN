---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26df8ea5d89eade705b2bead976f13be8f7b335e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412412"
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
result, err := graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).PostsById(&postId).ExtensionsById(&extensionId).Patch(options)


```