---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9f70383e9976966e4dda0e8eca98f621deeb129
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let response = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}')
    .version('beta')
    .get();

```