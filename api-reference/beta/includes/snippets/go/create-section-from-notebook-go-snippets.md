---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ac72bbbbe89d0310996c4ebbfc063911f662baf
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081726"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewOnenoteSection()
displayName := "Section name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.SectionsRequestBuilderPostOptions{
    Body: requestBody,
}
notebookId := "notebook-id"
result, err := graphClient.Me().Onenote().NotebooksById(&notebookId).Sections().Post(options)


```