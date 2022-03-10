---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16730c77f618ee8c507c67f5245515487fc9d970
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412326"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMailFolder()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.mailSearchFolder",
    "filterQuery": "contains(subject, 'Analytics')",
}
options := &msgraphsdk.MailFolderRequestBuilderPatchOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).Patch(options)


```