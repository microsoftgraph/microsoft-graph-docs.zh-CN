---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37e7d08b1d09222e0509e0cce837edea3877f7d4
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440277"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mobilityManagementPolicy = await client.api('/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020')
    .version('beta')
    .get();

```