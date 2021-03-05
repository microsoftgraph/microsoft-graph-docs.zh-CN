---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5589acfacd3542f80d595480dde17f9dc15b67a5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500489"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnualEvent = {
  allowedAudiences: "contacts"
};

let res = await client.api('/me/profile/anniversaries/{id}')
    .version('beta')
    .update(personAnnualEvent);

```