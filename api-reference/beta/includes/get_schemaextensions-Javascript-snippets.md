---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d2942f25f94042e2dde70e9f3876a5733e27e692
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446531"
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