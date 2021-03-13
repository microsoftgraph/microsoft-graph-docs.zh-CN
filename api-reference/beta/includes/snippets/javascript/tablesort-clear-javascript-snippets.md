---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7ad103631c7af18722d22bff81c9d5f365d6341
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear')
    .version('beta')
    .post();

```