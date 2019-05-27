---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dbb5aa9929e5e8fd1cabdc35434b297c0e3e0141
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessPeerToPeerActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```