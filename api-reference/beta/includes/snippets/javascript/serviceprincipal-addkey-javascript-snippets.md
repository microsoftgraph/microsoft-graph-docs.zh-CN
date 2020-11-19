---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 10993762f6db70a9b12aa37911629b986d9cc861
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addKey = {
    keyCredential: {
        type: "X509CertAndPassword",
        usage: "Sign",
        key: "MIIDYDCCAki..."
    },
    passwordCredential: {
        secretText: "MKTr0w1..."
    },
    proof:"eyJ0eXAiOiJ..."
};

let res = await client.api('/servicePrincipals/{id}/addKey')
    .version('beta')
    .post(addKey);

```