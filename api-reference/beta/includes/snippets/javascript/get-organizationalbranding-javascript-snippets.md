---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35bbec9841827199f12de21c288033f306ed0db1
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBranding = await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3/branding')
    .version('beta')
    .get();

```