---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73d2af41e2fea55630e14d9601862a7e62749338
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942751"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const keyCredential = {
    keyCredential: {
        type: 'AsymmetricX509Cert',
        usage: 'Verify',
        key: 'MIIDYDCCAki...'
    },
    passwordCredential: null,
    proof: 'eyJ0eXAiOiJ...'
};

await client.api('/applications/{id}/addKey')
    .version('beta')
    .post(keyCredential);

```