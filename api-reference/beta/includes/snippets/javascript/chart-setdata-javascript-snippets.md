---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3635c69450e0bcc1e5e1b4c4cead7a4734531820b0d88f5011440debf4dac71c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setData = {
  sourceData: 'sourceData-value',
  seriesBy: 'seriesBy-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData')
    .version('beta')
    .post(setData);

```