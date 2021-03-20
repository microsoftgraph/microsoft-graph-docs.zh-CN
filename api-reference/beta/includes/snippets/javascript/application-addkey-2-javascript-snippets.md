---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 080f26646b6f21559982a4b3e0fe889061b0fdfa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942756"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const keyCredential = {
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

await client.api('/applications/{id}/addKey')
    .version('beta')
    .post(keyCredential);

```