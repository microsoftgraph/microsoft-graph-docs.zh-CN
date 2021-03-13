---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b1a05de4487a85ce3c41ec3c4a432753a8f3e4b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801456"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailFolders = await client.api('/me/mailFolders/?includeHiddenFolders=true')
    .version('beta')
    .get();

```