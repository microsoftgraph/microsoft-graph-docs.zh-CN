---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5a831fa324a67e09018ef0f4aae0c4c2b6b8ab6b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingCurrencies/USD')
    .version('beta')
    .get();

```