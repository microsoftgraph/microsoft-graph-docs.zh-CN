---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c1908432bb0b570eca0895b0f2ccbe3cf627070c6f450c8a90f371f000fe82e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}')
    .version('beta')
    .delete();

```