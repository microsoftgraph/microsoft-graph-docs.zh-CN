---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 099ba66ed59bc025be6df00e580c0373fce7b075
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessReviews = await client.api('/accessReviews')
    .version('beta')
    .filter('businessFlowTemplateId eq \'6e4f3d20-c5c3-407f-9695-8460952bcc68\'')
    .skip(0)
    .top(100)
    .get();

```