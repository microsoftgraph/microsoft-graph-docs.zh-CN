---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c606428967ea24dfb860b4ea09492a1f745d1d2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let fido2Methods = await client.api('/me/authentication/fido2Methods')
    .version('beta')
    .get();

```