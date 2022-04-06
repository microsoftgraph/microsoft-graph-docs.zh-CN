---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e209a26e9b298f30dee171e8d91c4cf3af533851
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758821"
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
    scope: 'DelegatedPermissionGrant.ReadWrite.All'
};

await client.api('/oauth2PermissionGrants')
    .post(oAuth2PermissionGrant);

```