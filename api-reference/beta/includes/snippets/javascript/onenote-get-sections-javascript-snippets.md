---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 290e3b3e25e4ef39a3cf7faf1471a78cfb2b87a8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/sections')
    .version('beta')
    .get();

```