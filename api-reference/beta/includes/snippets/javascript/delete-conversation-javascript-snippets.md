---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed1dc857e6af1bf8c254a4c3d92d8a68a46f5cf5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/conversations/{id}')
    .version('beta')
    .delete();

```