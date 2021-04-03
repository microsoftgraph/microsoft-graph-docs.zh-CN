---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 837c5900cc07353ab645473ab7a22fe054f54ecd
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573163"
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