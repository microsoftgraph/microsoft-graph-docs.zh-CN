---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a6b012015b71d14ea2a82acc9380e345846690e
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appId: "65415bb1-9267-4313-bbf5-ae259732ee12"
};

let res = await client.api('/servicePrincipals')
    .post(servicePrincipal);

```