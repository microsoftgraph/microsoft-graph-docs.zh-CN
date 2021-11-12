---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61f95287cd50ebb1226068d04faea5ced1d54c1b328bc389a147d1dc49aafd1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104833"
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