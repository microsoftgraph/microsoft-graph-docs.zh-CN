---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fc517b676824b12f40f86b886323253ff38adce0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780270"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

await client.api('/groups/{id}/getMemberGroups')
    .post(string);

```