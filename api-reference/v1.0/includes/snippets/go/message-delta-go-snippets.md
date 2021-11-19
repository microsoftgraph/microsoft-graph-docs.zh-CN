---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05d175a2665c1046a70d306696743a1d46e1d2aa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084332"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "odata.maxpagesize=2"
}
options := &msgraphsdk.MessageRequestBuilderGetOptions{
    H: headers,
}
mailFolderId := "mailFolder-id"
messageId := "message-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).MessagesById(&messageId).Get(options)


```