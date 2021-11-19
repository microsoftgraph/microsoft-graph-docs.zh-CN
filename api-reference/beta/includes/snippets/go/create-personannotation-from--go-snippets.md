---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0053fe864d7970ea06b2aa72c51b62fc20288dfa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084048"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPersonAnnotation()
detail := msgraphsdk.NewItemBody()
requestBody.SetDetail(detail)
contentType := "text"
detail.SetContentType(&contentType)
content := "I am originally from Australia, but grew up in Moscow, Russia."
detail.SetContent(&content)
displayName := "About Me"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.NotesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Profile().Notes().Post(options)


```