---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8fd66bd2e493bb3ef6febb74a556e2f6a1fdd964
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440756"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```