---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b2e2e5f14edf4fab8f7d18a3bd405d971cbfc4c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800938"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let post = await client.api('/groups/{id}/threads/{id}/posts/{id}')
    .get();

```