---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1314586c74a460f62f78686b28bb5b2c016143de
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223072"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroupMember = {
  @odata.type: "#microsoft.graph.externalGroupMember",
  id: "1431b9c38ee647f6a",
  type: "group",
  identitySource: "external"
};

let res = await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .version('beta')
    .post(externalGroupMember);

```