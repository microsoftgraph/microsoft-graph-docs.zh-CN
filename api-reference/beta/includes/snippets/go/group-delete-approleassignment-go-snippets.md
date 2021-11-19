---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07e29abfc1bb9b079b5011896edfd2b960b9c6d2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095960"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.GroupsById(&groupId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete(options)


```