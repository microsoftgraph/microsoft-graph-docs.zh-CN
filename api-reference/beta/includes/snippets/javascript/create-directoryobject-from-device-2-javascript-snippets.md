---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 199aea3010ac48d2a7ff7c40f5fbea5cb6e2652e95c013fea493839859e4c168
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332519"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/directoryObjects/{id}'
};

await client.api('/devices/{id}/registeredUsers/$ref')
    .version('beta')
    .post(directoryObject);

```