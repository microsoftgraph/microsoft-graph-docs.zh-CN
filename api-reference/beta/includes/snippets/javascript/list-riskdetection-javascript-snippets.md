---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d0be37be4e95d7bb4a484d87e8b79ac91428a56
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "35725755"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/riskDetections')
    .version('beta')
    .get();

```