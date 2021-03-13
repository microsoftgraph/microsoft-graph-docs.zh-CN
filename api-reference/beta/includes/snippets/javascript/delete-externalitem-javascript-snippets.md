---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae15a2b30a0a044837d5bc16ecb2c9f0c4a397a9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788211"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/connections/contosohr/items/TSP228082938')
    .version('beta')
    .delete();

```