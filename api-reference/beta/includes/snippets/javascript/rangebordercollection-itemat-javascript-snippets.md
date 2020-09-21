---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 089153f356e9f41185ef9fe50ee3c5ea7bf7dff2
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636652"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  index: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/ItemAt')
    .version('beta')
    .post(workbookRangeBorder);

```