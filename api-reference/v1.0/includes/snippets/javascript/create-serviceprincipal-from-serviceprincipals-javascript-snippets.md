---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 363a51a913de3fb9e94a7afa66ad88248926dc07
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appId: "65415bb1-9267-4313-bbf5-ae259732ee12",
};

let res = await client.api('/serviceprincipals')
    .post(servicePrincipal);

```