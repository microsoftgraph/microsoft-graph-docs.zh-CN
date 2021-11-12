---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 832436a0fc8c569e75f94bf8cc29f0b68bae40d5c306e6767640f0fe6759d99f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278381"
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