---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3556ac3f5095f964863a88db22abf58cc7618c35
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/me/mailFolders/AAMkAGVmMDEzM/messages')
    .version('beta')
    .get();

```