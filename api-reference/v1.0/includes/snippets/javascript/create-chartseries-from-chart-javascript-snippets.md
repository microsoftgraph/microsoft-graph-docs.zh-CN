---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1193ac3a06ff66c952dd35c43976674b0a4c1c3d42319addf073c0f5c6eb0cef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  name: 'name-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series')
    .post(workbookChartSeries);

```