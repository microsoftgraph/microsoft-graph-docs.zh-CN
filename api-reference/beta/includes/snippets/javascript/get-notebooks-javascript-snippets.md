---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 282767f70d38c56f553f9b74bc545a4d3270b68b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notebooks = await client.api('/me/onenote/notebooks')
    .version('beta')
    .get();

```