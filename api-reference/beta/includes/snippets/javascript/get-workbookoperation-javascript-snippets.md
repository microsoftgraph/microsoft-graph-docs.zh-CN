---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c27712688a9ddf06741d9f9b9a111f82613ff5c3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806943"
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