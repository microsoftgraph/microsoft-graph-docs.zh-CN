---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb9121629bf1962c979325a48fe63fdc7b87a8e6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962967"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let passwordlessMicrosoftAuthenticatorAuthenticationMethod = await client.api('/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1')
    .version('beta')
    .get();

```