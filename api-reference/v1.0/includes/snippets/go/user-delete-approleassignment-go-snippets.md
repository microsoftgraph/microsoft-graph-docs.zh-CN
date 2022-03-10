---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e343c79ed5ce44c5f14851d1ecf8d00b91dc991c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412187"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
appRoleAssignmentId := "appRoleAssignment-id"
result, err := graphClient.UsersById(&userId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete(nil)


```