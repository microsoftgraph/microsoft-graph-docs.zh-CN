---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a5581a15cb5788725105cecf179bb9fc25d1bf25b9f0effb877226dd0bd8738
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/groups/{id}/transitivemembers/microsoft.graph.group')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .get();

```