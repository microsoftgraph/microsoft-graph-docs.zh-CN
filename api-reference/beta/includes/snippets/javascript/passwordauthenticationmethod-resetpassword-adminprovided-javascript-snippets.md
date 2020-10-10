---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b82f8853f38bef5853a77de3dee13949f180a759
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48417935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordResetResponse = {
  newPassword: "newPassword-value",
};

let res = await client.api('/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword')
    .version('beta')
    .post(passwordResetResponse);

```