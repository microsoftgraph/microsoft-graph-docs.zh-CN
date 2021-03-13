---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be57df571d919836df1ae42595dcf82490fb4562
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784903"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: 'Social events'
};

await client.api('/me/calendar')
    .version('beta')
    .update(calendar);

```