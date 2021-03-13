---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dfa14b47150eb8358ab18e79b7b250bdba34314
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskFolders = await client.api('/me/outlook/taskFolders')
    .version('beta')
    .get();

```