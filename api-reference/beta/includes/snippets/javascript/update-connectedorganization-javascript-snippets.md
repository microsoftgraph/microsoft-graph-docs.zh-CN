---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8f49fc880d02f3523d5496ae4deb8f066fe951c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectedOrganization = {
  displayName: 'Connected organization new name',
  description: 'Connected organization new description',
  state: 'configured'
};

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}')
    .version('beta')
    .update(connectedOrganization);

```