---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3aa05a40a39cbfcd95148138078a44208c344d1c
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLineFormat = {
  color: "color-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line')
    .version('beta')
    .update(workbookChartLineFormat);

```