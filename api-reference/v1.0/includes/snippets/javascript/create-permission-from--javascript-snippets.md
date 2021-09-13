---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a85e031470299c1d88d8c9a252635892b5aa9c8abc9fb1664afcd1c678abbf1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332328"
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