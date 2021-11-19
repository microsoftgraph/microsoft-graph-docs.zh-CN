---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4d06d55066f9760565670d48125b59e1d76908b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100942"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMailFolder()
displayName := "Weekly digests"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.mailSearchFolder",
    "includeNestedFolders": true,
    "sourceFolderIds":  []String {
        "AQMkADYAAAIBDAAAAA==",
    }
    "filterQuery": "contains(subject, 'weekly digest')",
}
options := &msgraphsdk.ChildFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).ChildFolders().Post(options)


```