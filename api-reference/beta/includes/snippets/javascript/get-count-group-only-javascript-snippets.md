---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16ea1219fbfa30af728e5e7627c0246b6a180327
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332942"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/memberOf/microsoft.graph.group/$count')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .get();

```