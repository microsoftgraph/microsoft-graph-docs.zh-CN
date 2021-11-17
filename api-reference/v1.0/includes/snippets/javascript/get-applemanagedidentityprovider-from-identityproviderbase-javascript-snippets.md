---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37be8bf520b6455266b16f8152d9f1ecdf6af692
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021421"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/Apple-Managed-OIDC')
    .get();

```