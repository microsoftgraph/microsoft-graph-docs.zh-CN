---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7dd327368713fd821dfde9316d18382d75135a56
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474553"
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