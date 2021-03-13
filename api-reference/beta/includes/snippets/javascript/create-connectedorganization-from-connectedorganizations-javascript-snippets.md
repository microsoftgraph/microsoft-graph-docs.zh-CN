---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daa56ec1f2c55653bc4091cc0b50334342fca054
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectedOrganization = {
  displayName: 'Connected organization name',
  description: 'Connected organization description',
  identitySources: [
    {
      '@odata.type': '#microsoft.graph.domainIdentitySource',
      domainName: 'example.com',
      displayName: 'example.com'
      }
  ],
  state: 'proposed'
};

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/')
    .version('beta')
    .post(connectedOrganization);

```