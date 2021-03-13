---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 02bcc19f2eac27534ca9b5d2d2e11d717863c7b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onenoteSection = await client.api('/me/onenote/sections/{id}')
    .version('beta')
    .get();

```