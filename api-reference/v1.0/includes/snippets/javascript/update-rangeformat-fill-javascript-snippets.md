---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e29c1825d7421738c1abe3d62a287e4bd2e4445b567ed1c171772df83b13f46
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: '#FF0000'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/fill')
    .update(workbookRangeFill);

```