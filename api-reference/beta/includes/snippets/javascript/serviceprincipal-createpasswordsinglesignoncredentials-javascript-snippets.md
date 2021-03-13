---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9684b0c40909f33f18b740ec2574e01cc4d69a36
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797345"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordSingleSignOnCredentialSet = {
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

await client.api('/servicePrincipals/{id}/createPasswordSingleSignOnCredentials')
    .version('beta')
    .post(passwordSingleSignOnCredentialSet);

```