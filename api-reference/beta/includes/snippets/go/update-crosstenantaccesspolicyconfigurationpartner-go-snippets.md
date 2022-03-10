---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4be6f3f5f6d1c7b0798a848910e63b64cdfb1934
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411681"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCrossTenantAccessPolicyConfigurationPartner()
inboundTrust := msgraphsdk.NewCrossTenantAccessPolicyInboundTrust()
requestBody.SetInboundTrust(inboundTrust)
isMfaAccepted := true
inboundTrust.SetIsMfaAccepted(&isMfaAccepted)
isCompliantDeviceAccepted := true
inboundTrust.SetIsCompliantDeviceAccepted(&isCompliantDeviceAccepted)
isHybridAzureADJoinedDeviceAccepted := true
inboundTrust.SetIsHybridAzureADJoinedDeviceAccepted(&isHybridAzureADJoinedDeviceAccepted)
options := &msgraphsdk.CrossTenantAccessPolicyConfigurationPartnerRequestBuilderPatchOptions{
    Body: requestBody,
}
crossTenantAccessPolicyConfigurationPartnerTenantId := "crossTenantAccessPolicyConfigurationPartner-tenantId"
result, err := graphClient.Policies().CrossTenantAccessPolicy().PartnersById(&crossTenantAccessPolicyConfigurationPartnerTenantId).Patch(options)


```