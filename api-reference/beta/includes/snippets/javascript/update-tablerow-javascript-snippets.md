---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b1465dda36922f243a15ecb1ad8ae78973dcde1342fd84a3fbf428964b1ae84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332274"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: 99,
  values: 'values-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .version('beta')
    .update(workbookTableRow);

```