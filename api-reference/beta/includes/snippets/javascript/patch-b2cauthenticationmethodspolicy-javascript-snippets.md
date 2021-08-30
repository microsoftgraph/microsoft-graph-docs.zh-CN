---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09987adec185b06ed5f904f2079c296e3f3014b7f5536b755493eff8e9cca3fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cAuthenticationMethodsPolicy = {
    isEmailPasswordAuthenticationEnabled: false,
    isUserNameAuthenticationEnabled: true,
    isPhoneOneTimePasswordAuthenticationEnabled: true
};

await client.api('/policies/b2cAuthenticationMethodsPolicy')
    .version('beta')
    .update(b2cAuthenticationMethodsPolicy);

```