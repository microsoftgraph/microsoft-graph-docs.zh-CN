---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cee713032c035b152cd4a8ac095dec3c7d29ef95
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/users/{id}/oauth2PermissionGrants')
    .version('beta')
    .get();

```