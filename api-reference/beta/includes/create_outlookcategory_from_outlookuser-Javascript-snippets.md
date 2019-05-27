---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f8f88da12bb483022e1c4399d52fbb490dcdb01d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
      displayName:"Project expenses",
      color:"preset9"
};

let res = await client.api('/me/outlook/masterCategories')
    .version('beta')
    .post({outlookCategory : outlookCategory});

```