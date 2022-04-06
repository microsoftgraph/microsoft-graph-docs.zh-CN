---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc0aedc6909d040a191ab953af710d60b2f2ea72
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758608"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const oAuth2PermissionGrant = {
    clientId: 'ef969797-201d-4f6b-960c-e9ed5f31dab5',
    consentType: 'AllPrincipals',
    resourceId: '943603e4-e787-4fe9-93d1-e30f749aae39',
    scope: 'DelegatedPermissionGrant.ReadWrite.All',
    startTime: '2022-03-17T00:00:00Z',
    expiryTime: '2023-03-17T00:00:00Z'
};

await client.api('/oauth2PermissionGrants')
    .version('beta')
    .post(oAuth2PermissionGrant);

```