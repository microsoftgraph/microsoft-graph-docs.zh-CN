---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d8d3d387b66873e8bda7ed5490223220a2f60a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/users/{id}'
};

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors/$ref')
    .version('beta')
    .post(directoryObject);

```