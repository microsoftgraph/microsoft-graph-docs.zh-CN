---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14b120b03fb04e57c390d6c6eabcecc615450005
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  id: 'id-value',
  height: 99,
  left: 99
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts')
    .post(workbookChart);

```