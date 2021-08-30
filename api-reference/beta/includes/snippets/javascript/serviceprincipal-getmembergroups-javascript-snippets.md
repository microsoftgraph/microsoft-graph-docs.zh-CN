---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9073560ff2055c728cf24854adfb26719b21122b36607e7eeb3c3198b857365
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/servicePrincipals/{id}/getMemberGroups')
    .version('beta')
    .post(string);

```