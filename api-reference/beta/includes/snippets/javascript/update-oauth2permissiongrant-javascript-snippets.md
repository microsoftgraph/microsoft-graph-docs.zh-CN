---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83ac454a3eddd80d3a2a7d0089550fd7391fa147
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797889"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const oAuth2PermissionGrant = {
  scope: 'scope-value'
};

await client.api('/oauth2PermissionGrants/{id}')
    .version('beta')
    .update(oAuth2PermissionGrant);

```