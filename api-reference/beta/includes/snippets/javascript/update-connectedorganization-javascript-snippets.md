---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c010daa5775a8df1c60eecee9a143ff6403450b
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectedOrganization = {
  displayName:"Connected organization new name",
  description:"Connected organization new description"
};

let res = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}')
    .version('beta')
    .update(connectedOrganization);

```