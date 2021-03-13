---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b34e1726c07596b1722687988f4f51d92f60ab3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794094"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolders = await client.api('/me/mailFolders')
    .version('beta')
    .get();

```