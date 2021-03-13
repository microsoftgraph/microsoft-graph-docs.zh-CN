---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9dc71fe8f33577f0bf982965e6742a246c217e7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786988"
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
      displayName: 'Foo App'
    }
  }]
};

await client.api('/sites/{sitesId}/permissions')
    .version('beta')
    .post(permission);

```