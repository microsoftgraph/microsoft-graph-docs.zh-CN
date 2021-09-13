---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bc4c6f8b00e9b2e09a730a9ec3c55f7f29613f5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identity = {
  id: 'e5477431-1038-484e-bf69-1dfedb97a110',
  type: 'group'
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .post(identity);

```