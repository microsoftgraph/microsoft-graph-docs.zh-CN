---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0a76d094fb41790ea1ba38c7bdabbac9340a8cb4ff95c1458195d914c283d58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  id: 'id-value',
  height: 99,
  left: 99
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts')
    .post(workbookChart);

```