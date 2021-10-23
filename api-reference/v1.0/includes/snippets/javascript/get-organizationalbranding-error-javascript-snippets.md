---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cc412db483eadcab2547a3607d4846e2adddd8f
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBranding = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .header('Accept-Language','0')
    .get();

```