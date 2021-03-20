---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6eb1c5fb454523fb98a966583e4db877b1210fa4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addKey = {
    keyCredential: {
        type: 'X509CertAndPassword',
        usage: 'Sign',
        key: 'MIIDYDCCAki...'
    },
    passwordCredential: {
        secretText: 'MKTr0w1...'
    },
    proof: 'eyJ0eXAiOiJ...'
};

await client.api('/servicePrincipals/{id}/addKey')
    .version('beta')
    .post(addKey);

```