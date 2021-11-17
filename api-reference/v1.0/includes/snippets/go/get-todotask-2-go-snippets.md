---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e76be7f4fbdb099170e9fd3bb6915a18758deea
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973598"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

todoTaskListId := "todoTaskList-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).Tasks().Get(options)


```