---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5534e8f54394a1f5ac5f0e1dbd82fe215370c3b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609285"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}')
    .version('beta')
    .get();

```