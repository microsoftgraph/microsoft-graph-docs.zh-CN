---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9078d30aae2335a8f2313a95956997b4326494c8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "#0000FF"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill')
    .version('beta')
    .update({workbookRangeFill : workbookRangeFill});

```