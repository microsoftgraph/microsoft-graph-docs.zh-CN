---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2cf72f245a20ac85e24fc647e5f3b1ea8fcf2aa4
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093639"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedAccessId := "privilegedAccess-id"
governanceRoleAssignmentRequestId := "governanceRoleAssignmentRequest-id"
result, err := graphClient.PrivilegedAccessById(&privilegedAccessId).RoleAssignmentRequestsById(&governanceRoleAssignmentRequestId).UpdateRequest(privilegedAccess-id, governanceRoleAssignmentRequest-id).Post()


```