---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9437f1c3e8f660df5383a78dbec91e1485eab62b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412198"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMailFolder()
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.MailFolderRequestBuilderPatchOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).Patch(options)


```