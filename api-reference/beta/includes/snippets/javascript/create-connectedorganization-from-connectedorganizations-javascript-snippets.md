---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca92e50b37480258bf6924d0f5435f7a503d798c
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47331064"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectedOrganization = {
  displayName:"Connected organization name",
  description:"Connected organization description",
  identitySources: [
    {
      @odata.type: "#microsoft.graph.domainIdentitySource",
      domainName: "example.com",
      displayName: "example.com"
      }
  ],
  state:"proposed"
};

let res = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/')
    .version('beta')
    .post(connectedOrganization);

```