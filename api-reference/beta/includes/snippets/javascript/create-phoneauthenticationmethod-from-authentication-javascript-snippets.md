---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a344f147f826179bcfc1e2a45656351e592d1c0e2194a29e0b2ca499943051b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104512"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const phoneAuthenticationMethod = {
  phoneNumber: '+1 2065555555',
  phoneType: 'mobile'
};

await client.api('/me/authentication/phoneMethods')
    .version('beta')
    .post(phoneAuthenticationMethod);

```