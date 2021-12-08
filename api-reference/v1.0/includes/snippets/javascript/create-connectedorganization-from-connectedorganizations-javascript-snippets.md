---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bc7b40fe1bbaa1463280dcac23471a27a1504bb
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347966"
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
    .post(connectedOrganization);

```