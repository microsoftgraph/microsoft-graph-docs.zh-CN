---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9345fd73eb0d2f8a89876986544c4db22b5eae3c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471709"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/errors')
    .version('beta')
    .get();

```