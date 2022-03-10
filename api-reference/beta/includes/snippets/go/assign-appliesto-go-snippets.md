---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45dfb548e33d2319f1d39a8728c272f501d29386
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411831"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}",
}
options := &msgraphsdk.AppManagementPolicyRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
appManagementPolicyId := "appManagementPolicy-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).AppManagementPoliciesById(&appManagementPolicyId).Post(options)


```