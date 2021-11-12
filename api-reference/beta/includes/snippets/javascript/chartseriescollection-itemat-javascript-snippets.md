---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d0bcbd8b793170a7493ffef0c3e57f5e72cf828a25df3f4f3b9f9100fae71b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902847"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  index: {
  }
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/ItemAt')
    .version('beta')
    .post(workbookChartSeries);

```