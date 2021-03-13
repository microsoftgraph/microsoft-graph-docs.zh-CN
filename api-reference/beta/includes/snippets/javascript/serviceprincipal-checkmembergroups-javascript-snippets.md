---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8efa037950c2af97279a903448274149b31640ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803688"
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
    .version('beta')
    .post(string);

```