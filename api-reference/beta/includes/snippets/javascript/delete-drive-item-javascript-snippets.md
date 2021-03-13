---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d20e17bfcac5fb61725a5b148e979ee355bafbc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799285"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{item-id}')
    .version('beta')
    .delete();

```