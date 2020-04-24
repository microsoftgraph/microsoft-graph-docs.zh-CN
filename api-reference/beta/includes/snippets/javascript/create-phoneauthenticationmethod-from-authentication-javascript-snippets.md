---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80dcca79f872554d23338eed14f168868831fa6f
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805705"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const phoneAuthenticationMethod = {
  phoneNumber: "+1 2065555555",
  phoneType: "mobile",
};

let res = await client.api('/me/authentication/phoneMethods')
    .version('beta')
    .post(phoneAuthenticationMethod);

```