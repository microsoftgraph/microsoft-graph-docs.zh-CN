---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 313f1e16de284cc3442a25722b661473fb806abe
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48417936"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword')
    .version('beta')
    .post();

```