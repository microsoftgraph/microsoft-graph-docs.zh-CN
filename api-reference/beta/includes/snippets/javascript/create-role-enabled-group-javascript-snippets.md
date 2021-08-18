---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c426347e53115a06f0c199d75adefd20ecb866c5928c466e121b8ea1c1ae079
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277446"
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