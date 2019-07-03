---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5a831fa324a67e09018ef0f4aae0c4c2b6b8ab6b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479062"
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