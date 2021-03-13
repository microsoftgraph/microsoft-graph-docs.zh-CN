---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d043f8b5e56abe0a8c02b619a1aed81417052c3b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/contactFolders/delta')
    .version('beta')
    .get();

```