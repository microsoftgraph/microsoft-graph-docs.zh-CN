---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6fc7e5d35dd119ace73046881945a7b12d24f362
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476800"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')')
    .get();

```