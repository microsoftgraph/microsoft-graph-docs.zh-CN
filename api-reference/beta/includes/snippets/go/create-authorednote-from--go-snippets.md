---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8188e28224f018e35a011f767bd7b15a5031458d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089241"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthoredNote()
content := msgraphsdk.NewItemBody()
requestBody.SetContent(content)
content := "String"
content.SetContent(&content)
contentType := "text"
content.SetContentType(&contentType)
options := &msgraphsdk.NotesRequestBuilderPostOptions{
    Body: requestBody,
}
subjectRightsRequestId := "subjectRightsRequest-id"
result, err := graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).Notes().Post(options)


```