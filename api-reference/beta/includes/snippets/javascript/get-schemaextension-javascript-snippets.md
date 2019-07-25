---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1a67d671b5ee87c33528fa1e42e82ef8788a1519
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/schemaExtensions/graphlearn_test')
    .version('beta')
    .get();

```