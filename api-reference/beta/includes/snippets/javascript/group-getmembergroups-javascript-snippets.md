---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87c99f1b1de0411b30670933647d60923854f2b0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790787"
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
    .version('beta')
    .post(string);

```