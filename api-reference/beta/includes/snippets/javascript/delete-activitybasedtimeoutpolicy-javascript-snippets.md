---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fa70316548a076a52d7e1d6902f010e473097ad
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475480"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/activityBasedTimeoutPolicies/{id}')
    .version('beta')
    .delete();

```