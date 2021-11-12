---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f90899e57c06df9fab384ffd5b3446dddae53f2929619aab0efdc23f1d8707cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273913"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartPoint = {
  index: {
  }
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt')
    .version('beta')
    .post(workbookChartPoint);

```