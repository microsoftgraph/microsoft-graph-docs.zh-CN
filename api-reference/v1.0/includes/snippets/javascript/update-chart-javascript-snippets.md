---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc49427031aa4a1f379e1545c19dca757efbc5bf5154e2d5cf9c54e04165dc3f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  height: 99,
  left: 99
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}')
    .update(workbookChart);

```