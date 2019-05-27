---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4488ae9b931f959119643b6a46aaa93d557f27fb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageStorage(period='D7')')
    .get();

```