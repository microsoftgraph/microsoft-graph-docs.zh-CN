---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbc5daebe3f0e3d52fab5b50bd3249b2a4f37608
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629801"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMobilityManagementPolicy()
complianceUrl := "https://portal.mg.contoso.com/?portalAction=Compliance"
requestBody.SetComplianceUrl(&complianceUrl)
discoveryUrl := "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc"
requestBody.SetDiscoveryUrl(&discoveryUrl)
termsOfUseUrl := "https://portal.mg.contoso.com/TermsofUse.aspx"
requestBody.SetTermsOfUseUrl(&termsOfUseUrl)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
}
mobilityManagementPolicyId := "mobilityManagementPolicy-id"
graphClient.Policies().MobileAppManagementPoliciesById(&mobilityManagementPolicyId).Patch(requestBody)


```