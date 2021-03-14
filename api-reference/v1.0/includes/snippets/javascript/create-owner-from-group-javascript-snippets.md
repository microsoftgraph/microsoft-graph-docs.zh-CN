---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac78379440d2058c121ec2c6f11bff9f6d0fa493
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/users/{id}'
};

await client.api('/groups/{id}/owners/$ref')
    .post(directoryObject);

```