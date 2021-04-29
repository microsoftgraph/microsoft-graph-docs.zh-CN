---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5427720dd839984ea152d020c8c4f7e14b9d58a3
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081576"
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