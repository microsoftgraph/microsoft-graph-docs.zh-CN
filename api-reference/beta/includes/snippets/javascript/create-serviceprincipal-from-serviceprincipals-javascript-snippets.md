---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 153f46c0e1a1f9f932a4aa2757dc35a95177e7bf2ce835033637332b61eba05f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164253"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appId: '65415bb1-9267-4313-bbf5-ae259732ee12',
};

await client.api('/servicePrincipals')
    .version('beta')
    .post(servicePrincipal);

```