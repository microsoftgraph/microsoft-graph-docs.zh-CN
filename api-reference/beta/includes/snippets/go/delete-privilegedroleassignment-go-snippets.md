---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da634d0914df4beeb63c05adf21314a98b0d71a2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315307"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedRoleAssignmentId := "privilegedRoleAssignment-id"
graphClient.PrivilegedRoleAssignmentsById(&privilegedRoleAssignmentId).Delete()


```