---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 447f72a3aa666add5f7135a81062b866a2459688
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903906"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/userFlowAttributes/{id}')
    .version('beta')
    .get();

```