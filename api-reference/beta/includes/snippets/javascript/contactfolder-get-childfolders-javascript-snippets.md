---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41ca2b4ea3c7e8df8b476aa49bf3500fb71227c6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783204"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/contactFolders/{id}/childFolders')
    .version('beta')
    .get();

```