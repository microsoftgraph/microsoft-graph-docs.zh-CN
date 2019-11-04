---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20835729913396a10fda90c62c4a7f36cc564db9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  use: "use-value",
  k: "application-secret-to-be-uploaded",
  nbf: 1508969811,
  exp: 1508973711
};

let res = await client.api('/trustFramework/keySets/{id}/uploadSecret')
    .version('beta')
    .post(trustFrameworkKey);

```