---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a19bcf3e7a2495623b3d8767be74eb6d9a662e83
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801538"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = The contents of the file goes here.;

await client.api('/me/drive/items/{item-id}/content')
    .version('beta')
    .put(stream);

```