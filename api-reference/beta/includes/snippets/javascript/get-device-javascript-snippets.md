---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b5534e8f54394a1f5ac5f0e1dbd82fe215370c3b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520211"
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