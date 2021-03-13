---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 623f0c420952887ca3ee1a390bfbc6b6dceb4a58
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775421"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}')
    .version('beta')
    .delete();

```