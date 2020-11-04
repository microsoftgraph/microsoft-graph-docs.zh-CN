---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cb07d22ca92ff302b7d1be8de92f3c49b54996a
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/userFlowAttributes')
    .version('beta')
    .get();

```