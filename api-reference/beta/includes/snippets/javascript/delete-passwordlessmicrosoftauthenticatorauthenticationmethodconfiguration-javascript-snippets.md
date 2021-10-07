---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ca4065647be558c97954db722c9c59c9ed8e7f2b4fa32c5d5d01f2860338f76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator')
    .version('beta')
    .delete();

```