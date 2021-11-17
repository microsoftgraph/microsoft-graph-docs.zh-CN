---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6744388dbb185ef62f0f91621e3dc0f58bcc892a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61010295"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleAssignmentScheduleRequestId := "unifiedRoleAssignmentScheduleRequest-id"
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequestsById(&unifiedRoleAssignmentScheduleRequestId).Get(options)


```