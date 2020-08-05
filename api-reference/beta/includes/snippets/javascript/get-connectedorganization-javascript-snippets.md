---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74645d63eb7f03527cecf1390685871e6b13aabb
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}')
    .version('beta')
    .get();

```