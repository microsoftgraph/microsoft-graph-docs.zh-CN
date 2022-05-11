---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20bbc9aabecf0ee56993d9fbd4b72a465336bbd2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327455"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
groupId := "groupId-value"
requestBody.SetGroupId(&groupId)
renameAs := "renameAs-value"
requestBody.SetRenameAs(&renameAs)
notebookId := "notebook-id"
result, err := graphClient.Me().Onenote().NotebooksById(&notebookId).CopyNotebook(notebook-id).Post(requestBody)


```