---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2942f25f94042e2dde70e9f3876a5733e27e692
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609964"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/schemaExtensions')
    .version('beta')
    .filter('id eq 'graphlearn_test'')
    .get();

```