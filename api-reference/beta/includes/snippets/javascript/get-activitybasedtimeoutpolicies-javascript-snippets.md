---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d28091e5d3bf4819af29f34fdb8d68ba3f41fb6428f0ea673d8dcbb999c37760
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let activityBasedTimeoutPolicies = await client.api('/policies/activityBasedTimeoutPolicies')
    .version('beta')
    .get();

```