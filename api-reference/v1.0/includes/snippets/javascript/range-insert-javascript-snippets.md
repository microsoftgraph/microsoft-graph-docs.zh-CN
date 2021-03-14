---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ec7c271712896b47159709b52fb9d2a86398aaa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
  shift: 'shift-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/insert')
    .post(workbookRange);

```