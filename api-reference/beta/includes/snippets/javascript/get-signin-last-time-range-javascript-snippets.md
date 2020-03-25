---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0891a6c803c213be8cf94700f5dcd948bd5740a5
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947178"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users?filter=signInActivity/lastSignInDateTime%20le%202019-06-01T00:00:00Z')
    .version('beta')
    .filter('signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z')
    .get();

```