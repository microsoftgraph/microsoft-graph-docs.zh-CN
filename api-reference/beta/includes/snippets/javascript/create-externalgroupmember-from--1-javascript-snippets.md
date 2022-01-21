---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f4fd629bd700f78c53280b62862ec8b3950f2cf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identity = {
  id: 'e811976d-83df-4cbd-8b9b-5215b18aa874',
  type: 'user',
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .version('beta')
    .post(identity);

```