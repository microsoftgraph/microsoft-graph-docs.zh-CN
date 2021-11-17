---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dbd1ef6e9866f106758c274340303ae5d031bcc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60976720"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

groupId := "group-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.GroupsById(&groupId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete(options)


```