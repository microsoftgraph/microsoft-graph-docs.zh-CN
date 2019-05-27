---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 271e61c11681b746daaad54b245e18f476b50060
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473720"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingCurrencies')
    .version('beta')
    .get();

```