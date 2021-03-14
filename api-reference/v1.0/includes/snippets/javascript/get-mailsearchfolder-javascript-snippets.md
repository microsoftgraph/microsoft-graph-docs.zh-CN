---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1afa907843f855655ce9c83a347b2d028d617444
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786002"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolder = await client.api('/me/mailFolders/AAMkAGVmMDEzN')
    .get();

```