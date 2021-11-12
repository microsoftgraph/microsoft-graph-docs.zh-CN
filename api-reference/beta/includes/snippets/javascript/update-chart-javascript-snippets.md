---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fc3efc28c62bc6f433199858e1169f974b09d7df4bf82463864b4b5e8bec44c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219273"
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
    .version('beta')
    .update(workbookChart);

```