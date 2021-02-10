---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4447c9c2fbe5d116f19d2d21341ab156f2742e8d
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179564"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews')
    .version('beta')
    .filter('businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68'')
    .skip(0)
    .top(100)
    .get();

```