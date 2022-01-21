---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24659555d1ca23c449b38eabb0375fff4a21b07b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137663"
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
    .version('beta')
    .post(identity);

```