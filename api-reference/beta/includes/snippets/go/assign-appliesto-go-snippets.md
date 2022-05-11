---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc43f99946446f181699b8ef239392b8b5bfb3b5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326610"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}",
}
servicePrincipalId := "servicePrincipal-id"
appManagementPolicyId := "appManagementPolicy-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).AppManagementPoliciesById(&appManagementPolicyId).Post(requestBody)


```