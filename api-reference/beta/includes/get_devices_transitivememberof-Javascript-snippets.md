---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dfdb4fecdca336d69e9d8f247bf213a712d21553
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472166"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```