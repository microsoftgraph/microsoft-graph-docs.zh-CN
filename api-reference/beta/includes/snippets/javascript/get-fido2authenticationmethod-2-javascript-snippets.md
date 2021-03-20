---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c606428967ea24dfb860b4ea09492a1f745d1d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953304"
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