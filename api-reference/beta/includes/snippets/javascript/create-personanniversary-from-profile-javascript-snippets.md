---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8eefca5c67e26582286a3b2e617c517a32694cb1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500480"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnualEvent = {
  type: "birthday",
  date: "1980-01-08"
};

let res = await client.api('/me/profile/anniversaries')
    .version('beta')
    .post(personAnnualEvent);

```