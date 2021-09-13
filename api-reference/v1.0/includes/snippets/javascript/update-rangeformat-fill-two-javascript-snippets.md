---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5fd8c5b19dfafd79774fd7d3ec519083bb5c6ff9dcc8527c4582c2e571c16cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: '#00FF00'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/fill')
    .update(workbookRangeFill);

```