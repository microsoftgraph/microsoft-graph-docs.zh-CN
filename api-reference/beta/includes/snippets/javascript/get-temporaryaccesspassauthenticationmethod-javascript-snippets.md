---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b09fd1029c341ebbbd48df650383126702e4f447
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443159"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let temporaryAccessPassAuthenticationMethod = await client.api('/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods/05267842-25b2-4b21-8abd-8e4982796f7f')
    .version('beta')
    .get();

```