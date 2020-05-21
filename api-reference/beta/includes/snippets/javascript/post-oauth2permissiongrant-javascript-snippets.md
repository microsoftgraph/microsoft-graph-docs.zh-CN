---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b1884ce0b6212018b570427b150fcb9d0f1af28
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333679"
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
  scope: "scope-value",
  startTime: "2016-10-19T10:37:00Z",
  expiryTime: "2016-10-19T10:37:00Z"
};

let res = await client.api('/oauth2PermissionGrants')
    .version('beta')
    .post(oAuth2PermissionGrant);

```