---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d548f4ad300a0f297765bc5a36660be0a533885f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethod = await client.api('/me/authentication/methods/{id}')
    .version('beta')
    .get();

```