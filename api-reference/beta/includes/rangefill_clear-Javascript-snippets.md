---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 95d82d8bb9f3677c8813dd46f6d3aa1d6847b855
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear')
    .version('beta')
    .post();

```