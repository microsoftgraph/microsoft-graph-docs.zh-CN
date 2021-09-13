---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ea8e42c59e0e396fe28b141bcb827b9bbf8664ea429f61839019995b3fa9041
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903882"
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
    .update(oAuth2PermissionGrant);

```