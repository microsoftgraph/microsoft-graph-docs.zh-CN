---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c29fd053460e3b77b1ef0116a707dee977f53149
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803068"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

await client.api('/groups/{id}/getMemberObjects')
    .version('beta')
    .post(string);

```