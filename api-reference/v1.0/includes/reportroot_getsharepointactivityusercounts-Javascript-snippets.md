---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 992bc74ed82a311cdaa6c6374f093749a373ba19
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477185"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityUserCounts(period='D7')')
    .get();

```