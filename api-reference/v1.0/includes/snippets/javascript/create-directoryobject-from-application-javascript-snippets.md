---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ebf2b85165a1b66917f4403fae15b0decedbcbd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792886"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
};

await client.api('/applications/{id}/owners/$ref')
    .post(directoryObject);

```