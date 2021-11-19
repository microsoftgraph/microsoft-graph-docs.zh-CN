---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c936ba447663725e21648d3968242199102779e9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089661"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedRoleAssignmentId := "privilegedRoleAssignment-id"
result, err := graphClient.PrivilegedRoleAssignmentsById(&privilegedRoleAssignmentId).Get(options)


```