---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23bffc3a61fc81d0ad49cbbc7113e7d0c0adacb8
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1')
    .version('beta')
    .get();

```