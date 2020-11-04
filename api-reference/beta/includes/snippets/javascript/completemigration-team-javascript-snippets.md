---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6383156f9780cf30f7963f8251c97259e5c671f
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903574"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/completeMigration')
    .version('beta')
    .post();

```