---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9f7eb034b8512d3e08a2dfbcf9eee1691754700506a62595af4dba8883eabd6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219510"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookOperation = await client.api('/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}')
    .version('beta')
    .get();

```