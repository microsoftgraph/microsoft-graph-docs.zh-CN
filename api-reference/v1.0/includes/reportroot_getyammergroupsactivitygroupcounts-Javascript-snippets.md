---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 735cd4b244a1d97dfd3bf3a7a4044c6496c409be
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityGroupCounts(period='D7')')
    .get();

```