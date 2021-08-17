---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b773b5dd3b70a15f674f1144126dc3b327bb64bb
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368857"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020')
    .version('beta')
    .delete();

```