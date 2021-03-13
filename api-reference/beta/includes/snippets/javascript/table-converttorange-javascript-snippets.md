---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 865d545ea2cc9587f46305ce58d5e4aef300b8a1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange')
    .version('beta')
    .post();

```