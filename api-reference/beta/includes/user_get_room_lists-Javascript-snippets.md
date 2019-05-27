---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ecd8776d521e84c950e9562b12ef3e8c412483c2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/findRoomLists')
    .version('beta')
    .get();

```