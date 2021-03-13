---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 837c67681eeb27f06624778352271d2ec61fffb6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let microsoftAuthenticatorMethods = await client.api('/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods')
    .version('beta')
    .get();

```