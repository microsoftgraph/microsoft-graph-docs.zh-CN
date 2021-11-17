---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 119f1468cf3145b1bcb3df05f11f9c6f3253a860
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989993"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

plannerTaskId := "plannerTask-id"
result, err := graphClient.Planner().TasksById(&plannerTaskId).Get(options)


```