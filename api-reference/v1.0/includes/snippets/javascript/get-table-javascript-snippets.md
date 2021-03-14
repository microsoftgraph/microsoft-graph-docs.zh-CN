---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c8a174f6f19d752631403e0f8c11e2a10c824a1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785679"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTable = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}')
    .get();

```