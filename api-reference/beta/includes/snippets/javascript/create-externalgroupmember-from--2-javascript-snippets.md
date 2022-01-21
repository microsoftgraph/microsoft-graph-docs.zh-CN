---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6245b5348ea97adb0f3897d9aa385bef31912d4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137669"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identity = {
  id: 'e5477431-1038-484e-bf69-1dfedb97a110',
  type: 'externalGroup',
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .version('beta')
    .post(identity);

```