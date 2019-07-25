---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f12a47f2883fdd42ef1d2e257f65328ae548d553
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708895"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/mute')
    .version('beta')
    .post(CommsOperation);

```