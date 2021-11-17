---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7084a9f1fc4183a811f5e41e443435756d2ac647c5ed3a21e794c8e936e9ec6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const updatePasswordSingleSignOnCredentials = {
  id: '5793aa3b-cca9-4794-679a240f8b58',
  credentials: [
    {
      fieldId: 'param_username',
      value: 'myusername',
      type: 'username'
    },
    {
      fieldId: 'param_password',
      value: 'pa$$w0rd',
      type: 'password'
    }
  ]
};

await client.api('/servicePrincipals/{id}/updatePasswordSingleSignOnCredentials')
    .version('beta')
    .post(updatePasswordSingleSignOnCredentials);

```