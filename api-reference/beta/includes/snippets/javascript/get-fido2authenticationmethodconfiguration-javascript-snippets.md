---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b83da6274bce7fe3146c2241fbe5cd9385acb0a523329bfbf13a325e8aaacc39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273895"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2')
    .version('beta')
    .get();

```