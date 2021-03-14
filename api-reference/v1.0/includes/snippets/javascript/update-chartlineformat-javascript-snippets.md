---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c27520805928c3cd693420a527c3a41daad8891
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795790"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLineFormat = {
  color: 'color-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line')
    .update(workbookChartLineFormat);

```