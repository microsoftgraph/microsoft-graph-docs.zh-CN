---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf305c2d5fd3a767a98f4e45981db2f84c0d6c167f12ba3ba0aeefe31b9c893a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278957"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviderBase = await client.api('/identity/identityProviders/Apple-Managed-OIDC')
    .version('beta')
    .get();

```