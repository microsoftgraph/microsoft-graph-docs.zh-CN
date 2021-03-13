---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4cc8065e85b84c1dde725d7b12e58f8a06ac823
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795881"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threads = await client.api('/groups/{id}/threads')
    .version('beta')
    .get();

```