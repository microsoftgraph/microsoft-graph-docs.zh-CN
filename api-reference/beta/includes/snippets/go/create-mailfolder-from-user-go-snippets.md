---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd246f5dc97b087b1b11cedb302a66796a0ecc61
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985163"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewMailFolder()
displayName := "Clutter"
requestBody.SetDisplayName(&displayName)
isHidden := true
requestBody.SetIsHidden(&isHidden)
options := &msgraphsdk.MailFoldersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().MailFolders().Post(options)


```