---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 806ecc13204aab8d0b2e5a196d5642b4f521ee2f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007893"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
groupId := "groupId-value"
requestBody.SetGroupId(&groupId)
renameAs := "renameAs-value"
requestBody.SetRenameAs(&renameAs)
options := &msgraphsdk.CopyNotebookRequestBuilderPostOptions{
    Body: requestBody,
}
notebookId := "notebook-id"
result, err := graphClient.Me().Onenote().NotebooksById(&notebookId).CopyNotebook().Post(options)


```