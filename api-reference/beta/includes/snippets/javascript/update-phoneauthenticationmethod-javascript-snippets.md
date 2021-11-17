---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 916ad325d029a49233b56d369ec71142d62bc75e7e910e14eae13ff8ee3c48d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const phoneAuthenticationMethod = {
  phoneNumber: '+1 2065555554',
  phoneType: 'mobile',
};

await client.api('/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7')
    .version('beta')
    .put(phoneAuthenticationMethod);

```