---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7001ffc283efefa17cc3aa3b0693d735a066095
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61010309"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleAssignmentScheduleInstanceId := "unifiedRoleAssignmentScheduleInstance-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleInstancesById(&unifiedRoleAssignmentScheduleInstanceId).Get(options)


```