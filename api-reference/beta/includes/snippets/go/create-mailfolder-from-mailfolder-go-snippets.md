---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2440338d7239e05a85e488b272e9bebf94b9b85b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090987"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMailFolder()
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isHidden := true
requestBody.SetIsHidden(&isHidden)
options := &msgraphsdk.ChildFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).ChildFolders().Post(options)


```