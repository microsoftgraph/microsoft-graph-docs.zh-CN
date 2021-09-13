---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b4e49538233b95c15411d75c730733556d24fb1f8a5295ac4993423294bb14c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id':'https://graph.microsoft.com/v1.0/users/alexd@contoso.com'
};

await client.api('/groups/{id}/rejectedSenders/$ref')
    .post(directoryObject);

```