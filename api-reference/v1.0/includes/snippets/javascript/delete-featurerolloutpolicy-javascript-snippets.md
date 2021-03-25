---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f90a4fe1f216c09a7f6c420aa9dc8fa6c76b7f1
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c')
    .delete();

```