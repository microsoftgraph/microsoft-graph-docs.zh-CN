---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0b330af128f75affed54d37a40e8b47b1e7de6ec
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737237"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartGridlines = {
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines')
    .update({workbookChartGridlines : workbookChartGridlines});

```