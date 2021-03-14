---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b953c7a4e936aa71fba63a52a1b80971d341ca0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
    'groupIds-value'
  ]
};

await client.api('/servicePrincipals/{id}/checkMemberGroups')
    .post(string);

```