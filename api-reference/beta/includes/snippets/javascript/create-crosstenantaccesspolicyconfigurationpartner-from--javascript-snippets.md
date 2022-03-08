---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1daea12d78c75bfb0cd97da38b9e4d0524d00bb3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335841"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const crossTenantAccessPolicyConfigurationPartner = {
  tenantId: '3d0f5dec-5d3d-455c-8016-e2af1ae4d31a',
  b2bDirectConnectOutbound: 
  {
    usersAndGroups: 
    {
      accessType: 'blocked',
      targets: [
        {
            target: '6f546279-4da5-4b53-a095-09ea0cef9971',
            targetType: 'group'
        }
      ]
    }
  },
  b2bDirectConnectInbound: 
  {
    applications: 
    {
      accessType: 'allowed',
      targets: [
        {
            target: 'Office365',
            targetType: 'application'
        }
      ]
    }
  }
};

await client.api('/policies/crossTenantAccessPolicy/partners')
    .version('beta')
    .post(crossTenantAccessPolicyConfigurationPartner);

```