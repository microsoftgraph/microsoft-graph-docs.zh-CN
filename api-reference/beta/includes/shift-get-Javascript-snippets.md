---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d2fbfe55aaa8cdb9628a6df27d3e53866719fd12
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .version('beta')
    .get();

```