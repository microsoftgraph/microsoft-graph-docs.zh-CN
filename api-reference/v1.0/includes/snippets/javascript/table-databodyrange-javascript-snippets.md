---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2392b99afd16597e5acc1364985f4f6bf6b348e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/dataBodyRange')
    .get();

```