---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 12daaa229d9f88558c1b38dd1797966e5e690696
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438481"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/11014/assignmentCategories/19002')
    .version('beta')
    .delete();

```