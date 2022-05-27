---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 671aa08e7c6f64442aa3424be3f430aa7e4596cea061c82d678183db1e2ea0cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref')
    .version('beta')
    .delete();

```