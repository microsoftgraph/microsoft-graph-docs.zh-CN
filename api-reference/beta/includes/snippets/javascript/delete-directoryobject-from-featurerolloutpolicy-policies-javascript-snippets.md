---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69c69df6c177d73f95bafff6b84a57f1081a6c4c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508705"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c/appliesTo/2441b489-4f12-4882-b039-8f6006bd66da/$ref')
    .version('beta')
    .delete();

```