---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6625817a05b63a5c7753a72f590a61e9bfd0f05a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782852"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartDataLabels = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels')
    .get();

```