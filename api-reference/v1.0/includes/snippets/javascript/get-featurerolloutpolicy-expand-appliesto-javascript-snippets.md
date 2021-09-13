---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2edc299c9f919ef7e6dd85b40ffb51b935e2051d51aa18e883cdc3d9f57a22bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let featureRolloutPolicy = await client.api('/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c')
    .expand('appliesTo')
    .get();

```