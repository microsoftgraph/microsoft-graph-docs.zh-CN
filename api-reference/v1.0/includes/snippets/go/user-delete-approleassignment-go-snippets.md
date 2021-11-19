---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23188b73b37d32db859d049a994138e660250f7f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083826"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.UsersById(&userId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete(options)


```