---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce120fe180e30a0e12a3da5f29848453da3cc24ed6a5bcc40ad76140d1226389
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: 'Group with designated owner and members',
  displayName: 'Operations group',
  groupTypes: [
  ],
  mailEnabled: false,
  mailNickname: 'operations2019',
  securityEnabled: true,
  'owners@odata.bind': [
    'https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2'
  ],
  'members@odata.bind': [
    'https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc',
    'https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14'
  ]
};

await client.api('/groups')
    .post(group);

```