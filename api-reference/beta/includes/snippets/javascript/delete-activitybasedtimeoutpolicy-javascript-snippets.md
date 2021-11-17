---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97f0d0e2a2e08529755ab35bd2b8e8a8827f02e516c23a418fab4accc2b63caa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902613"
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