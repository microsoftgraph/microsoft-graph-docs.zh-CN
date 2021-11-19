---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a35c33e592b6943e85198c3781e2807fb6d54fd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088395"
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
options := &msgraphsdk.MobilityManagementPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
mobilityManagementPolicyId := "mobilityManagementPolicy-id"
graphClient.Policies().MobileAppManagementPoliciesById(&mobilityManagementPolicyId).Patch(options)


```