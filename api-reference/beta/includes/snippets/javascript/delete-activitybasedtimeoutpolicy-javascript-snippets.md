---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b3668b83c2d1c50d7c2fcbd6f731c7ee2416689
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/activityBasedTimeoutPolicies/{id}')
    .version('beta')
    .delete();

```