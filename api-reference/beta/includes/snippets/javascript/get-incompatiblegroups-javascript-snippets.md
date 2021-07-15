---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7dac8f08e529ff8e5724cf4d4de84f2c0c87c56
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let incompatibleGroups = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups')
    .version('beta')
    .get();

```