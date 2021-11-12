---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e64391086e97de8e5c23941ac57038cb18189ffbd0a4ae03bd167d49d66112cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104885"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  type: 'ColumnStacked',
  sourceData: 'A1:B1',
  seriesBy: 'Auto'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add')
    .version('beta')
    .post(workbookChart);

```