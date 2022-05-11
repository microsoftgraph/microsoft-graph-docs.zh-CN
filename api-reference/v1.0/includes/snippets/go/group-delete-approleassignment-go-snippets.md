---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f399bf389435077ff88673f4ccb1fd0a6ab95676
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327324"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.GroupsById(&groupId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete()


```