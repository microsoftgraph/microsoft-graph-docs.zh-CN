---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e3b1349681ab125a1696067211dbc52ade68253
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223166"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroup = {
  @odata.type: "#microsoft.graph.externalGroup",
  id: "31bea3d537902000",
  displayName: "Contoso Marketing",
  description: "The product marketing team"
};

let res = await client.api('/external/connections/contosohr/groups')
    .version('beta')
    .post(externalGroup);

```