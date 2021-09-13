---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b85586a5c49fc691ce8b78bab0b12e2a95d70dc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022637"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identity = {
  id: '1431b9c38ee647f6a',
  type: 'externalGroup',
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .post(identity);

```