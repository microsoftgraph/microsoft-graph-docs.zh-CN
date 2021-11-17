---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 472b9ae481c0f317ef39bbc3cacc07a88e655e05a0be00080f86d036afac338a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215689"
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