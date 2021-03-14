---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28c321f4e83e31c6cdd8639ae93c69f0cd19741c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778454"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  'members@odata.bind': [
    'https://graph.microsoft.com/v1.0/directoryObjects/{id}',
    'https://graph.microsoft.com/v1.0/directoryObjects/{id}',
    'https://graph.microsoft.com/v1.0/directoryObjects/{id}'
    ]
};

await client.api('/groups/{group-id}')
    .update(group);

```