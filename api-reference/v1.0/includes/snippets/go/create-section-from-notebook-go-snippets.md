---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de3e992ea5f580f0223ed8f8ece092064a1c18f1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023314"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewOnenoteSection()
displayName := "Section name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.SectionsRequestBuilderPostOptions{
    Body: requestBody,
}
notebookId := "notebook-id"
result, err := graphClient.Me().Onenote().NotebooksById(&notebookId).Sections().Post(options)


```