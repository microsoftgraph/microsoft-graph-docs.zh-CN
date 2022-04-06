---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f1ccddd06d0d64e8a08e1b068e949e4e7e7fbd2
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758842"
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
    .update(oAuth2PermissionGrant);

```