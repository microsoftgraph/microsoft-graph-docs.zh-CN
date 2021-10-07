---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c1176a9ec46edc861ad96c3a0cbd3e6999ecc4c3e9a4c2e8fa5b3473a835421
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105613"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator')
    .version('beta')
    .get();

```