---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6a30ad373ba0ed02de0d10ae871c39e3d6b4fdf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805696"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let phoneMethods = await client.api('/me/authentication/phoneMethods')
    .version('beta')
    .get();

```