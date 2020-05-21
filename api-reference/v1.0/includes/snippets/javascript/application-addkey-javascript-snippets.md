---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb608fd616451991836c0d30ddc63e09ac1fd378
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const keyCredential = {
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

let res = await client.api('/applications/{id}/addKey')
    .post(keyCredential);

```