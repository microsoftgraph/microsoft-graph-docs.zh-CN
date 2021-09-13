---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f98eac6b5bf2474f8f5b7e0fe33c58a4f79fa0638f9667d81bf1f2c04f5da6a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrantPolicy = await client.api('/policies/permissionGrantPolicies/microsoft-user-default-low')
    .get();

```