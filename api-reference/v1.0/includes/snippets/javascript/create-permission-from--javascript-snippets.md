---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e5f46ad2e3807e59a49bdb7546ee8f5057e686c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: ['write'],
  grantedToIdentities: [{
    application: {
      id: '89ea5c94-7736-4e25-95ad-3fa95f62b66e',
      displayName: 'Contoso Time Manager App'
    }
  }]
};

await client.api('/sites/{sitesId}/permissions')
    .post(permission);

```