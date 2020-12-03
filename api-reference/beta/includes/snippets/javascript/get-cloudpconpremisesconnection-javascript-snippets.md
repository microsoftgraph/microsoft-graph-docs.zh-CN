---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ccec172e852b544474cbbf77d883fa93caaeae1
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521689"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{id}')
    .version('beta')
    .get();

```