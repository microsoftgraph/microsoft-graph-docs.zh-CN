---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb950522637a626d5c253dde24feec0d9bde4ba4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801750"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartLegend = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
    .version('beta')
    .get();

```