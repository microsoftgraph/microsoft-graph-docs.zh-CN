---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1fb08ef1da9d09df8fc8fd1a18f09507814b7e96
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476002"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscription = {
   expirationDateTime:"2016-11-22T18:23:45.9356913Z"
};

let res = await client.api('/subscriptions/{id}')
    .version('beta')
    .update({subscription : subscription});

```