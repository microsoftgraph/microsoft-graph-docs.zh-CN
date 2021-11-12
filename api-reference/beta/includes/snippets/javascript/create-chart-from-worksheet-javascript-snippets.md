---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aecc1ab5ab6d92160404131d4ebeb89691194c094e98280b2e67750b77d745c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  id: 'id-value',
  height: 99,
  left: 99
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts')
    .version('beta')
    .post(workbookChart);

```