---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a1c65c06400b1987d7dbcc103fd97358ce4d5e2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787671"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartDataLabels = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels')
    .version('beta')
    .get();

```