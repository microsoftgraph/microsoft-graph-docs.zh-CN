---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 070167ef80518e562aa2b7e91b3b0471acbd72cd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007753"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

privilegedRoleAssignmentId := "privilegedRoleAssignment-id"
graphClient.PrivilegedRoleAssignmentsById(&privilegedRoleAssignmentId).Delete(options)


```