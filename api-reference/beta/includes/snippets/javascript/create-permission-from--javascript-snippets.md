---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b275e40724c7613a7c0c25e13a60170db628980c297cbc135914874e23aefda
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
   roles: [
      'write'
   ],
   grantedToIdentities: [
      {
         application: {
            id: '89ea5c94-7736-4e25-95ad-3fa95f62b66e',
            displayName: 'Contoso Time Manager App'
         }
      }
   ]
};

await client.api('/sites/{sitesId}/permissions')
    .version('beta')
    .post(permission);

```