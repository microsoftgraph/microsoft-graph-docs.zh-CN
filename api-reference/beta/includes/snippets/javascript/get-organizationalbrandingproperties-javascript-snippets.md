---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8deee373a7f4bdd18344219cd2fe678cc235289
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBrandingLocalization = {
    backgroundColor:"#00000F",
    id: "fr"
};

let res = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations')
    .version('beta')
    .post(organizationalBrandingLocalization);

```