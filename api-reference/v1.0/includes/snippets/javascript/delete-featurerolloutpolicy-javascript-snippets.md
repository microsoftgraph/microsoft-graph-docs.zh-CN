---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8481ece8319c8554b33e04977194e614647aa22e9249501276496584e24cea53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c')
    .delete();

```