---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 102113e7c2e3ac9b7547f2a2109f78520d36c3ea
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473958"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser(on='allowedRequestor')')
    .version('beta')
    .get();

```