---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a087f5c315f3cb594582df78eabbbe0bafcfba95
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736713"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "color-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .update({workbookRangeFill : workbookRangeFill});

```