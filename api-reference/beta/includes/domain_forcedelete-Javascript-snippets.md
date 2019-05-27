---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cbffeceb7f1572ccc91517881096a3e39f7e4106
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437074"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forceDelete = {
  disableUserAccounts: true
};

let res = await client.api('/domains/contoso.com/forceDelete')
    .version('beta')
    .post(forceDelete);

```