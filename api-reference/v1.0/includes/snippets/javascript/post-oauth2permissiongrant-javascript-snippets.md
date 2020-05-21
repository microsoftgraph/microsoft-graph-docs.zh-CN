---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3d03c05e8b56c84c3efa4af365d2d21e8aa1416
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const oAuth2PermissionGrant = {
  clientId: "clientId-value",
  consentType: "consentType-value",
  principalId: "principalId-value",
  resourceId: "resourceId-value",
  scope: "scope-value"
};

let res = await client.api('/oauth2PermissionGrants')
    .post(oAuth2PermissionGrant);

```