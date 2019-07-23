---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4c908b25cd18cf48c4653f3acac743c5afa6afe7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "Group with designated owner and members",
  displayName: "Operations group",
  groupTypes: [
    "Unified"
  ],
  mailEnabled: true,
  mailNickname: "operations2019",
  securityEnabled: false,
  owners@odata.bind: [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  members@odata.bind: [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
};

let res = await client.api('/groups')
    .version('beta')
    .post({group : group});

```