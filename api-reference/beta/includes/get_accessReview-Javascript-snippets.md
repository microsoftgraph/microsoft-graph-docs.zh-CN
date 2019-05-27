---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef056e74ac90300062cb0ec631d1a2b3b8e7aa66
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d')
    .version('beta')
    .get();

```