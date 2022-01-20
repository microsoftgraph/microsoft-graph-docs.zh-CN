---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa6d4e613da269967df18efd9b0fc840fd1dbc0d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113283"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
linkedResource_v2Id := "linkedResource_v2-id"
graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).LinkedResourcesById(&linkedResource_v2Id).Delete(nil)


```