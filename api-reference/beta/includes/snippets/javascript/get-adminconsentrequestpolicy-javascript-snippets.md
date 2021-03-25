---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 210f4bcb27a065b79870fb41e174e6fc38c1a0ce
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let adminConsentRequestPolicy = await client.api('/policies/adminConsentRequestPolicy')
    .version('beta')
    .get();

```