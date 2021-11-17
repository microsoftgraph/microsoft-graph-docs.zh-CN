---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f57b835c96b719c2a190d8a80aaf1381b5179a7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023398"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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