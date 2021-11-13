---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b441823c49d88d58fff1d7ee5a4ac71478e58371
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignments = await client.api('/education/classes/{id}/assignments')
    .version('beta')
    .get();

```