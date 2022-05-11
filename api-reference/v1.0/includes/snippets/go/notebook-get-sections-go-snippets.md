---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00d60134a30fec1f503fb2c22a607ee6e5c40217
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328042"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

notebookId := "notebook-id"
result, err := graphClient.Me().Onenote().NotebooksById(&notebookId).Sections().Get()


```