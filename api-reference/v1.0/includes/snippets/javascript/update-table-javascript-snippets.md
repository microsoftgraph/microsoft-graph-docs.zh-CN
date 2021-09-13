---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76bbef8c2d9ea71b1d15c321d818611db956bd3b6acdc9028647ea605406c364
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220370"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  name: 'name-value',
  showHeaders: true,
  showTotals: true,
  style: 'style-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}')
    .update(workbookTable);

```