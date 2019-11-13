---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16d48fff794dc19c4b70d5ee3e1badc9281d9de7
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302398"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/participants')
    .version('beta')
    .get();

```