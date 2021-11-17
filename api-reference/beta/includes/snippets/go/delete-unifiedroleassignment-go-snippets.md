---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8bfa44638d5fd50ad3a47e3303f848a2a19e229
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976916"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

unifiedRoleAssignmentId := "unifiedRoleAssignment-id"
graphClient.RoleManagement().Directory().RoleAssignmentsById(&unifiedRoleAssignmentId).Delete(options)


```