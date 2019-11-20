---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a7442f7a7dce326d3b08df74863471629dd41b2
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747921"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordSingleSignOnCredentialSet = {
  id: "5793aa3b-cca9-4794-679a240f8b58",
  credentials: [
    {
      fieldId: "param_username",
      value: "myusername",
      type: "username"
    },
    {
      fieldId: "param_password",
      value: "pa$$w0rd",
      type: "password"
    }
  ]
};

let res = await client.api('/servicePrincipals/{id}/createPasswordSingleSignOnCredentials')
    .version('beta')
    .post(passwordSingleSignOnCredentialSet);

```