---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a60af826cc5c4941d18566919f90fd50bab38616
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004548"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

userActivityId := "userActivity-id"
activityHistoryItemId := "activityHistoryItem-id"
graphClient.Me().ActivitiesById(&userActivityId).HistoryItemsById(&activityHistoryItemId).Put(options)


```