---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d89fa1758e91b3ad12249ac1a75209a80b41a71
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id':'https://graph.microsoft.com/v1.0/users/alexd@contoso.com'
};

await client.api('/groups/{id}/acceptedSenders/$ref')
    .post(directoryObject);

```