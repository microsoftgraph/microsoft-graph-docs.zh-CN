---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9078d30aae2335a8f2313a95956997b4326494c8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461718"
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