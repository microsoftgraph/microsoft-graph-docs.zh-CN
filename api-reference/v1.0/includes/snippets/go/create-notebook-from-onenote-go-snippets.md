---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22de5f24f0ae1dac9a4b52b1821e41ff839eb1c3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029398"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewNotebook()
displayName := "My Private notebook"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.NotebooksRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().Onenote().Notebooks().Post(options)


```