---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2360e955d4f0cb7808ee82e9beba5da9916993c8
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904113"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/userFlowAttributes/{id}')
    .version('beta')
    .delete();

```