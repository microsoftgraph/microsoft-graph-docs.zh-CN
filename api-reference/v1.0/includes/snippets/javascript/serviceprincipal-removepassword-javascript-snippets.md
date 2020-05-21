---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b2385d92e64491a1761ba7fa68fe1d5c44f828b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336586"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removePassword = {
    keyId: "f0b0b335-1d71-4883-8f98-567911bfdca6"
};

let res = await client.api('/servicePrincipals/{id}/removePassword')
    .post(removePassword);

```