---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97a44b127c0e8472204f5bb8eb14ca9e1bcf77bde13cd8dbce85de129c5f84b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277876"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/microsoftAuthenticator')
    .get();

```