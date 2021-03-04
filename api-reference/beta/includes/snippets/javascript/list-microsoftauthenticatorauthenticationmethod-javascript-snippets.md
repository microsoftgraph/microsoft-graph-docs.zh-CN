---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90659366806365fe0371b8fe44d62c0b018edac3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods')
    .version('beta')
    .get();

```