---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c135e7027b8deb23926f0e0c7a2554f7098f9607
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011681"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewMobilityManagementPolicy()
complianceUrl := "https://portal.uem.contoso.com/?portalAction=Compliance"
requestBody.SetComplianceUrl(&complianceUrl)
discoveryUrl := "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc"
requestBody.SetDiscoveryUrl(&discoveryUrl)
termsOfUseUrl := "https://portal.uem.contoso.com/TermsofUse.aspx"
requestBody.SetTermsOfUseUrl(&termsOfUseUrl)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
}
options := &msgraphsdk.MobilityManagementPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
mobilityManagementPolicyId := "mobilityManagementPolicy-id"
graphClient.Policies().MobileDeviceManagementPoliciesById(&mobilityManagementPolicyId).Patch(options)


```