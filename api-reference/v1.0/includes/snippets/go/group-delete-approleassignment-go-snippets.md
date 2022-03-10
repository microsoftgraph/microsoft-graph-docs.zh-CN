---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef6cb102efd844bef347615159acc75124dfe407
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412207"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
appRoleAssignmentId := "appRoleAssignment-id"
result, err := graphClient.GroupsById(&groupId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete(nil)


```