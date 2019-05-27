---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4dad99e10e1eebd8131f15709eabb51eac2cdfb6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473230"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels')
    .version('beta')
    .get();

```