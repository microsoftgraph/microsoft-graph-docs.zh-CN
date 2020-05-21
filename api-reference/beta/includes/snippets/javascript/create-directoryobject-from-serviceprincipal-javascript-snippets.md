---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3797d194ab0a2c69388b7c01388f0b750f16f462
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333474"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    @odata.id: "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
};

let res = await client.api('/servicePrincipals/{id}/owners/$ref')
    .version('beta')
    .post(directoryObject);

```