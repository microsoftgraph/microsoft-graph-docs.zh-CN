---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84847d168262ee9bb23e14ff90ab6ba9d7a6d5f2
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337146"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/entitlementManagement/assignmentRequests/filterByCurrentUser(on='target')')
    .get();

```