---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd511516cd3e1b14f2ca405cc64a5840db99bffe
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694427"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
claimsMappingPolicyId := "claimsMappingPolicy-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).ClaimsMappingPoliciesById(&claimsMappingPolicyId).$ref().Delete()


```