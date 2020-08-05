---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b066c6ff00ad25cb642ecee86a557a7ed528e889
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566558"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations')
    .version('beta')
    .get();

```