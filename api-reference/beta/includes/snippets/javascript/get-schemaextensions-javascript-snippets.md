---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d2942f25f94042e2dde70e9f3876a5733e27e692
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521541"
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