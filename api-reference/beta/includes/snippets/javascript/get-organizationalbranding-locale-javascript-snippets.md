---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3924d3dea18ab23d9699273e3321cb64e5c9f1f
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996263"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBranding = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .version('beta')
    .header('Accept-Language','fr-FR')
    .get();

```