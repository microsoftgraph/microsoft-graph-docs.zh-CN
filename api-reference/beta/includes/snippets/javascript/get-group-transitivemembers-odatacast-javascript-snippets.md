---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad61b109766a9a9c2c3597e6d8caa17c3c384ec0
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/groups/{id}/transitivemembers/microsoft.graph.group')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .get();

```