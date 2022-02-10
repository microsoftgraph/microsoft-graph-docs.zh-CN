---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e965055cd164f06d6b6c2f1ca224658aea805da
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519284"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

baseTaskListId := "baseTaskList-id"
graphClient.Me().Tasks().ListsById(&baseTaskListId).Delete(nil)


```