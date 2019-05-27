---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 10469783cfb156c2bd21eaf80194b07ed0780a5c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/masterCategories')
    .version('beta')
    .get();

```