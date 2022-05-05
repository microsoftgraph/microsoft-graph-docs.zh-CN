---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 577e635963e8a8cb2fccce4881cf2418e88febdc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204983"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleEligibilityScheduleId := "unifiedRoleEligibilitySchedule-id"
result, err := graphClient.RoleManagement().Directory().RoleEligibilitySchedulesById(&unifiedRoleEligibilityScheduleId).Get(nil)


```