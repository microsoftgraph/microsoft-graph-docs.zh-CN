---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be503795847df23a21f5224a01fefe91e89fcee6
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('endswith(mail,'a@contoso.com'),')
    .orderby('userPrincipalName ')
    .get();

```