---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61cb02df657b2d0d91e21038d91f3f13d58c655d
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336473"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/memberOf/$count')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .get();

```