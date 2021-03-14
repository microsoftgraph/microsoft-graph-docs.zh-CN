---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b81c2770515667d890733e9312d59df8fb253d48
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartGridlines = {
  visible: true
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines')
    .update(workbookChartGridlines);

```