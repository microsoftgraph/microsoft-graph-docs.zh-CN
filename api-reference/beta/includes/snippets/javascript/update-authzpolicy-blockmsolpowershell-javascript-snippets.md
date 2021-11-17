---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c1cc031b299878b9c519c48631ee27fcea31c40b73d600d0f8b9cfba69c8f5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903172"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   blockMsolPowerShell: true
};

await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```