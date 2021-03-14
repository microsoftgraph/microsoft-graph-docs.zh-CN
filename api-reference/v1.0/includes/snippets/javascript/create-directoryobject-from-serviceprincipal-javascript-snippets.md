---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6feff04fba029a1ec17a1e3830f611a31f2ece44
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785006"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
};

await client.api('/servicePrincipals/{id}/owners/$ref')
    .version('beta')
    .post(directoryObject);

```