---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 498feffb77ea2f6664de24079c8bf1489d89def4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804341"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnualEvent = {
  allowedAudiences: 'contacts'
};

await client.api('/me/profile/anniversaries/{id}')
    .version('beta')
    .update(personAnnualEvent);

```