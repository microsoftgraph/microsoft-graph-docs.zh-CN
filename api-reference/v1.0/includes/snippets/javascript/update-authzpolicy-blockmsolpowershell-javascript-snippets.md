---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6ab59f38c2007663e0f32c44613ddbce5b74c24431759a45a886f1acf858a0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277583"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   blockMsolPowerShell: true
};

await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```