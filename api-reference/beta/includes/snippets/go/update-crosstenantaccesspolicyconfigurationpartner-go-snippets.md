---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b351ef0ae5eadcc74f77b8d0369704ce63a1a84
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327469"
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
crossTenantAccessPolicyConfigurationPartnerTenantId := "crossTenantAccessPolicyConfigurationPartner-tenantId"
graphClient.Policies().CrossTenantAccessPolicy().PartnersById(&crossTenantAccessPolicyConfigurationPartnerTenantId).Patch(requestBody)


```