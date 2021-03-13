---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6607b272f77aec6ea3ec17ad1ade0f384b94589
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790967"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnualEvent = {
  type: 'birthday',
  date: '1980-01-08'
};

await client.api('/me/profile/anniversaries')
    .version('beta')
    .post(personAnnualEvent);

```