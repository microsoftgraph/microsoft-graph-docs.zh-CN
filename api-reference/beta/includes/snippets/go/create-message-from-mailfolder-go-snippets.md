---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 483fa04b31eb17e166f83521eaa7b58d79efea89
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328710"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
receivedDateTime, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
requestBody.SetReceivedDateTime(&receivedDateTime)
sentDateTime, err := time.Parse(time.RFC3339, "2016-10-19T10:37:00Z")
requestBody.SetSentDateTime(&sentDateTime)
hasAttachments := true
requestBody.SetHasAttachments(&hasAttachments)
subject := "subject-value"
requestBody.SetSubject(&subject)
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
contentType := ""
body.SetContentType(&contentType)
content := "content-value"
body.SetContent(&content)
bodyPreview := "bodyPreview-value"
requestBody.SetBodyPreview(&bodyPreview)
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).Messages().Post(requestBody)


```