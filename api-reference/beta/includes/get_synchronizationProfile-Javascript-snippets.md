---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0a8ac90e5f534082931e2e4c1799c288c6953b30
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445796"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}')
    .version('beta')
    .delete();

```