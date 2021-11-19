---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07df7e473e4acaa41535f3fc5c47f93f43a85ac1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103175"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
webUrl := "webUrl value"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.GetNotebookFromWebUrlRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Onenote().Notebooks().GetNotebookFromWebUrl().Post(options)


```