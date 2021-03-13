---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5cce9ad086f9e8a2e8eef9d2fbf6959c9cb4c5ad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oAuth2PermissionGrant = await client.api('/oauth2PermissionGrants/{id}')
    .version('beta')
    .get();

```