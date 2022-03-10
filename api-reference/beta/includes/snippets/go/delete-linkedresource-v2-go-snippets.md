---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 720f16d1676caf010ed3f698044e7cfaf1cd3f01
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412296"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
linkedResource_v2Id := "linkedResource_v2-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).LinkedResourcesById(&linkedResource_v2Id).Delete(nil)


```