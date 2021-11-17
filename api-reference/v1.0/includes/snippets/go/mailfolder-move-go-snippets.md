---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 873958a7070230be91a6ff0ecffa8b2a6fd95c7b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992954"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
destinationId := "destinationId-value"
requestBody.SetDestinationId(&destinationId)
options := &msgraphsdk.MoveRequestBuilderPostOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).Move().Post(options)


```