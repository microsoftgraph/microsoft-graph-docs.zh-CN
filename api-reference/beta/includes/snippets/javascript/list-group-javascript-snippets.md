---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a623df65a95e659e11c10386b6b7e8891ca6234
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let includedGroups = await client.api('/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups')
    .version('beta')
    .get();

```