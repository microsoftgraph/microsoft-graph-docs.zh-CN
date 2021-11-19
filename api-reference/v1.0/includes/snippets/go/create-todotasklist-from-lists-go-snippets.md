---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb170f9460877d165b5e45131ac084ccd861de31
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085047"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTodoTaskList()
displayName := "Travel items"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ListsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Todo().Lists().Post(options)


```