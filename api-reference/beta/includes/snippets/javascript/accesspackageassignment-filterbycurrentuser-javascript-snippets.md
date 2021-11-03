---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a80f71f9d9c56d055381859880ecec628affdc9a1aa6ae360acb0a94e6d58575
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignments/filterByCurrentUser(on='target')')
    .version('beta')
    .get();

```