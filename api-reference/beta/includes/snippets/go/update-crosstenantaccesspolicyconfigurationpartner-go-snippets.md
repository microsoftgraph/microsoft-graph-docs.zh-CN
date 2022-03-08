---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dcd567d5485f0bddb43e1e9a2199c87fc9e2679
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336184"
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
graphClient.Policies().CrossTenantAccessPolicy().PartnersById(&crossTenantAccessPolicyConfigurationPartnerTenantId).Patch(options)


```