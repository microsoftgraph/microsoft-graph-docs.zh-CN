---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f9a61c0499be2113fea1c619e8e82575dd8ef77
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777753"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .version('beta')
    .delete();

```