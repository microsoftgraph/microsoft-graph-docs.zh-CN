---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa08753b399e2ffc08f35eb37e21e069175f0cf1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803614"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let temporaryAccessPassMethods = await client.api('/me/authentication/temporaryAccessPassMethods')
    .version('beta')
    .get();

```