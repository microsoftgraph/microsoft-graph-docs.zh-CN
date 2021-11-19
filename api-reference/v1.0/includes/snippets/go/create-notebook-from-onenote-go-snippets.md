---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb9ab64f5ce484923e96c5e9ca220e900e2a218b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096807"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNotebook()
displayName := "My Private notebook"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.NotebooksRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Onenote().Notebooks().Post(options)


```