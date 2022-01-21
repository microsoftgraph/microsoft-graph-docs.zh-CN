---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9b901a16dd3e7dd7a5f1d5d2a556dd8a166a1bc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarView = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z')
    .version('beta')
    .get();

```