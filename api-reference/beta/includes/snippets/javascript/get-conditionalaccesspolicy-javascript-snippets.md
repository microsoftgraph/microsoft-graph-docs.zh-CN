---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6135e7bd294a4ddb95ac42c722cbd4fd2afd0299
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conditionalAccessPolicy = await client.api('/identity/conditionalAccess/policies/{id}')
    .version('beta')
    .get();

```