---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4565f25809e5237e0cd43e3ca5e4e04623d83c9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808614"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartGridlines = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines')
    .get();

```