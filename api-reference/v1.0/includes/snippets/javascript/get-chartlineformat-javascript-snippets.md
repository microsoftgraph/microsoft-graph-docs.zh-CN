---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7a3664673a613fe299f4c201fc08824e0c27105
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartLineFormat = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line')
    .get();

```