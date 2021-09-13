---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66dbac501d9ec8990b9553f2ecbfece2a0861ed4790ca29303ba900f9048935c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: 3
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt')
    .post(workbookTableColumn);

```