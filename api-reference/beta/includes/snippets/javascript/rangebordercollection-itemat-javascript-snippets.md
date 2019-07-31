---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e1ccd54b07b8b847d331dab8f6ca27fb4bc54aae
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727757"
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
    .post({workbookRangeBorder : workbookRangeBorder});

```