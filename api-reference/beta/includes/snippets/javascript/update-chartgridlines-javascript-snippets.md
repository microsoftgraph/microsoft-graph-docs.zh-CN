---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7a5654ca14ef1b1b2ff50c7a54b0151937428ff4b6818c2bf48e975a8aa511c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartGridlines = {
  visible: true
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines')
    .version('beta')
    .update(workbookChartGridlines);

```