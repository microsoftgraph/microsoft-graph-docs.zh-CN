---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ff7084f953d8f5d56624a3f33113a61411ec04b384b7f38f95539aab2c6bf2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartAxis = {
  majorUnit: {
  },
  maximum: {
  },
  minimum: {
  }
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis')
    .version('beta')
    .update(workbookChartAxis);

```