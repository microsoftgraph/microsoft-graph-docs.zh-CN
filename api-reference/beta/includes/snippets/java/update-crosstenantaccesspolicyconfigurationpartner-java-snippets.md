---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aa06cc91fe80d25c3e4fc4c16f839db05a49039
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336198"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CrossTenantAccessPolicyConfigurationPartner crossTenantAccessPolicyConfigurationPartner = new CrossTenantAccessPolicyConfigurationPartner();
CrossTenantAccessPolicyInboundTrust inboundTrust = new CrossTenantAccessPolicyInboundTrust();
inboundTrust.isMfaAccepted = true;
inboundTrust.isCompliantDeviceAccepted = true;
inboundTrust.isHybridAzureADJoinedDeviceAccepted = true;
crossTenantAccessPolicyConfigurationPartner.inboundTrust = inboundTrust;

graphClient.policies().crossTenantAccessPolicy().partners("90e29127-71ad-49c7-9ce8-db3f41ea06f1")
    .buildRequest()
    .patch(crossTenantAccessPolicyConfigurationPartner);

```