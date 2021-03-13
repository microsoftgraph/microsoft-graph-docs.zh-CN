---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31bf6a7d2127f3c17ca0acd1de6c55e5df7cc370
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786435"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/users/{id}'
};

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors/$ref')
    .version('beta')
    .post(directoryObject);

```