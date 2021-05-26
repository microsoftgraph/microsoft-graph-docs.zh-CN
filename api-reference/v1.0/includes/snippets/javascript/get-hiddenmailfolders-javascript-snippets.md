---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b1a05de4487a85ce3c41ec3c4a432753a8f3e4b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666203"
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