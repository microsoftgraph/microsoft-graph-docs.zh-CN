---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3746caf01f0cce4cb3a420ef725dee94e8c352eb84405e8ec338ee8003acfba6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartPoint = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/{point-id}')
    .get();

```