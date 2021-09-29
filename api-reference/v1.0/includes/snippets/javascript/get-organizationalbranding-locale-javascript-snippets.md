---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0782d3bd0681bb2db3cf90825d90154f2e11b170
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997073"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBranding = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .header('Accept-Language','fr-FR')
    .get();

```