---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 092dba62f98c495acf11cb676d6aa62e6c6f3538
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796237"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personAward = await client.api('/me/profile/awards/{id}')
    .version('beta')
    .get();

```