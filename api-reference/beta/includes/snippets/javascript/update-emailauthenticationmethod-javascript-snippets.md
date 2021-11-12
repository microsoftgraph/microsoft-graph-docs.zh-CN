---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 586eb18476f2fac034434782540adacd668d032b4b94fac13be5e172ca6cf75a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const emailAuthenticationMethod = {
  emailAddress: 'kim@contoso.com'
};

await client.api('/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f')
    .version('beta')
    .put(emailAuthenticationMethod);

```