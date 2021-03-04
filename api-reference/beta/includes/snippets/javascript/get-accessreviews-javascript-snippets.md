---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d23123bb08517a5c46a044c80af501d10f95d45
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews')
    .version('beta')
    .filter('businessFlowTemplateId eq \'6e4f3d20-c5c3-407f-9695-8460952bcc68\'')
    .skip(0)
    .top(100)
    .get();

```