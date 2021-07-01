---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f32a0d710a07fa573f0e016d13959faefc1e0bff
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209691"
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
    .post(group);

```