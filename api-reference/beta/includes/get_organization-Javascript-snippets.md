---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 26cfd7e7bc104a6fbbccc9994b29e8d70956c6d0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448158"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/organization')
    .version('beta')
    .get();

```