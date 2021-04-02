---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb3165702a2a7545511c526a5c36e3af8241a3a1
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let featureRolloutPolicy = await client.api('/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c')
    .version('beta')
    .get();

```