---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cab634ad0a63566e8edda7748239f90a0a50c00
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languages = await client.api('/me/profile/languages')
    .version('beta')
    .get();

```