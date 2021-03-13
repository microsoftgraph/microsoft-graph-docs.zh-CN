---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aa6e7dc748a48b92266edd613c4900437cb9a17
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793516"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/servicePrincipals/{id}/oauth2PermissionGrants')
    .version('beta')
    .get();

```