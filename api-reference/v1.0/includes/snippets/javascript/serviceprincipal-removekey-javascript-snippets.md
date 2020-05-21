---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffac099d5a91139f47068a4b9875cc7da355a9bc
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removeKey = {
    keyId: "f0b0b335-1d71-4883-8f98-567911bfdca6",
    proof:"eyJ0eXAiOiJ..."
};

let res = await client.api('/serviceprincipals/{id}/removeKey')
    .post(removeKey);

```