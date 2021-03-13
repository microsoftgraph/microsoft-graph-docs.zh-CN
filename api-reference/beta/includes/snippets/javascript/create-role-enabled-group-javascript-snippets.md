---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b3d502a0b927548f31196d3b621ce7092be10e2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: 'Group assignable to a role',
  displayName: 'Role assignable group',
  groupTypes: [
    'Unified'
  ],
  isAssignableToRole: true,
  mailEnabled: true,
  securityEnabled: true,
  mailNickname: 'contosohelpdeskadministrators',
  visibility: 'Private'
};

await client.api('/groups')
    .version('beta')
    .post(group);

```