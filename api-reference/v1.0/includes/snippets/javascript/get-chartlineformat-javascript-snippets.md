---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2649d18251d9f2f3a749ad8ffa8629916b34142ab71e437e8b9f5946e5760add
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartLineFormat = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line')
    .get();

```