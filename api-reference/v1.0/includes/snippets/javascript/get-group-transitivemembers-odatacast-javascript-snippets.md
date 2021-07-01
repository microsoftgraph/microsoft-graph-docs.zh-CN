---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cb6ae029644b51b1663319620c4b4a1ce5bd572
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/groups/{id}/transitivemembers/microsoft.graph.group')
    .header('ConsistencyLevel','eventual')
    .get();

```