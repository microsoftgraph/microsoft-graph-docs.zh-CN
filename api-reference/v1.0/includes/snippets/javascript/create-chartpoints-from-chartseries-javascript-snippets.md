---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f383bc839b893be5d817cab1f147f29f6edb31cb953ce07c5724df573577cea1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409755"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartPoint = {
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points')
    .post(workbookChartPoint);

```