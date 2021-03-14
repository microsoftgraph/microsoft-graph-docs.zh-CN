---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43018dce205f9e69f607aa14950dd59a70380827
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let children = await client.api('/drives/{drive-id}/items/{item-id}/children')
    .get();

```