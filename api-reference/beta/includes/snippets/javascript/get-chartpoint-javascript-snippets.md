---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d88ac92d29ad30a483bf1207364a5a31a4be2a6d42b3a0922697706bf90b3b86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartPoint = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/{undefined}')
    .version('beta')
    .get();

```