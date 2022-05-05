---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4e7ad57b1be3d9c6162fea7a3e9ccbcf42efd91
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordResetResponse = {
    newPassword: 'Cuyo5459'
};

await client.api('/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword')
    .version('beta')
    .post(passwordResetResponse);

```