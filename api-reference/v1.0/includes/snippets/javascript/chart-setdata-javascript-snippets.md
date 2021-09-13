---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 462fb85a0f2c4d5f6e6604ad87bdb2b8029ab14a9831e1bd3e50fa6a6c37a350
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902302"
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
    .post(setData);

```