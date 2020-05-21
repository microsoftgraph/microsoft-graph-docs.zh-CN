---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae0a6aa70844c82f1f5011e97370c5ec9c381278
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332922"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members/microsoft.graph.user/$count')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .get();

```