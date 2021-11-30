---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ea7cda584624652195d280b7681c15f85e2e7959294801d3e668fee016f4c92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221341"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordResetResponse = {
  newPassword: 'newPassword-value',
};

await client.api('/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword')
    .version('beta')
    .post(passwordResetResponse);

```