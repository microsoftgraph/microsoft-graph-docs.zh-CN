---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18963eb910e4fd3f1eaff07bdca60305a4b3a04c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784377"
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