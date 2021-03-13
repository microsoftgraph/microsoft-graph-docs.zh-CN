---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 449cc25b6715f825eb219361ddf9a521efcf74a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784734"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/autofitRows')
    .version('beta')
    .post();

```