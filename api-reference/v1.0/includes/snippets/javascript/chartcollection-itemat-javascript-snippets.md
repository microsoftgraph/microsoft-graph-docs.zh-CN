---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e446cb60c899b4eaa71d5dd4eda683b54404e7a1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  index: 8
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt')
    .post({workbookChart : workbookChart});

```