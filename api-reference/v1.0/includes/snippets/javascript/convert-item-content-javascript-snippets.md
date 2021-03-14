---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d36a00d42a7e94dce5e607583967d53566dc9cc8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788283"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/drive/items/{item-id}/content?format=%7Bformat%7D')
    .get();

```