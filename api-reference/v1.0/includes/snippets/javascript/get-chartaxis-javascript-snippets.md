---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7df585c2ee444e4549a7621e79f8bc29a7a89cf4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartAxis = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis')
    .get();

```