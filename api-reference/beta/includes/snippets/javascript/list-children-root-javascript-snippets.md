---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d456c3b8447a2142cf45891e6e425b95bc752b0e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796785"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/me/drive/root/children')
    .version('beta')
    .get();

```