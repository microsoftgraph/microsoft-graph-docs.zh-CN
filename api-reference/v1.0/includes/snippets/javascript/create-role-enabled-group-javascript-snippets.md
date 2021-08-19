---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cc16e0527f6ff12ac99ba058b9131eb8ff99473256bfd8f9f18074a70271e40
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278536"
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