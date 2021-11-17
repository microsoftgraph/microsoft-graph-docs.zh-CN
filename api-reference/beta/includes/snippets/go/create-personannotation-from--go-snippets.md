---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8b4f747fcd235b22f037a073189e2cfe940597d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980046"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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