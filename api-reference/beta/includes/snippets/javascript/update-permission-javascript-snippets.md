---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 463ccd487bdd565dea875416aa85970d4eb57eb7412c6f85b11bb7362ec43ccf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: [ 'read' ]
};

await client.api('/me/drive/items/{item-id}/permissions/{perm-id}')
    .version('beta')
    .update(permission);

```