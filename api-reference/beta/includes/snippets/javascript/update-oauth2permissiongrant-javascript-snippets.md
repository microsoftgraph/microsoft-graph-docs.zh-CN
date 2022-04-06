---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ee583a0e97078659d00994e0f7a5b439e28842f
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const oAuth2PermissionGrant = {
    scope: 'User.ReadBasic.All Group.ReadWrite.All'
};

await client.api('/oauth2PermissionGrants/l5eW7x0ga0-WDOntXzHateQDNpSH5-lPk9HjD3Sarjk')
    .version('beta')
    .update(oAuth2PermissionGrant);

```