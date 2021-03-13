---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c46a79f31d2cb89d6a3e9481867303f29a7c23a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791537"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let history = await client.api('/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history')
    .version('beta')
    .get();

```