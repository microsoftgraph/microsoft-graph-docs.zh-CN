---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f402ac6d523d956218787ca5110766cecf0b1fb7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442884"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/LastCell')
    .version('beta')
    .get();

```