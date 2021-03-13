---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72c8450b7bbb317f022aed5ec6c9db1ff5eeb0d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770901"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columnDefinition = await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}')
    .version('beta')
    .get();

```