---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea7d86fe668dd77138d79e326e5f85901f6f1b51
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412615"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewWebUrlRequestBody()
webUrl := "webUrl value"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.GetNotebookFromWebUrlRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Onenote().Notebooks().GetNotebookFromWebUrl().Post(options)


```