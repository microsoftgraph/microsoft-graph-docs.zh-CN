---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4093275c4181c7290da77ad06d85995f9a853cb
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411804"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
appRoleAssignmentId := "appRoleAssignment-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).AppRoleAssignedToById(&appRoleAssignmentId).Delete(nil)


```