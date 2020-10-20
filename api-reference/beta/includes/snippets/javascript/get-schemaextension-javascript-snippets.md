---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a67d671b5ee87c33528fa1e42e82ef8788a1519
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618583"
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