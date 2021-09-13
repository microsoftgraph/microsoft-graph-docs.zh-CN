---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81608168a34232ee7c0fee18512ef5e0ee214fc1a0d77b606b2acdb6a5642b58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLineFormat = {
  color: 'color-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line')
    .update(workbookChartLineFormat);

```