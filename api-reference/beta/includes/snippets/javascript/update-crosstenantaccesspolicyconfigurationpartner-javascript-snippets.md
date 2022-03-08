---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57ebae651e1238ddab7aa4b71118f957921fb797
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336205"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const crossTenantAccessPolicyConfigurationPartner = {
  inboundTrust: 
  {
    isMfaAccepted: true,
    isCompliantDeviceAccepted: true,
    isHybridAzureADJoinedDeviceAccepted: true
  }
};

await client.api('/policies/crossTenantAccessPolicy/partners/90e29127-71ad-49c7-9ce8-db3f41ea06f1')
    .version('beta')
    .update(crossTenantAccessPolicyConfigurationPartner);

```