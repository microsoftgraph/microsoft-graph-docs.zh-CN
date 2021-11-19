---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7afacd111ba92ae05fa3a9835ae27a5749adcb13
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098298"
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
graphClient.Me().MailFoldersById(&mailFolderId).Patch(options)


```