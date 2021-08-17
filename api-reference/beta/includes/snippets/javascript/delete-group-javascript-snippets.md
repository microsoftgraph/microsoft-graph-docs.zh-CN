---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e26ceebfc6df344c2fa2cbbf08f892bfef32322
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef/$ref')
    .version('beta')
    .delete();

```