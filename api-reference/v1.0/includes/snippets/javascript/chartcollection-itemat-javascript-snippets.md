---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29d2477e28e9f96c0ec4eb8bd60faba7bf838bf8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  index: 8
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt')
    .post(workbookChart);

```