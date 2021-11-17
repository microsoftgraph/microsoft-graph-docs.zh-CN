---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7becebfb45123f08a5ae746a4dbeabb28b4f5ba2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029454"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

notebookId := "notebook-id"
result, err := graphClient.Me().Onenote().NotebooksById(&notebookId).Get(options)


```