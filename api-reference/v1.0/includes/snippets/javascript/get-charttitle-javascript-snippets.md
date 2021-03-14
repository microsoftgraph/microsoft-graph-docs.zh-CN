---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b39dc40ba41ad6dcb6adad24a0305a6adc5789c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartTitle = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title')
    .get();

```