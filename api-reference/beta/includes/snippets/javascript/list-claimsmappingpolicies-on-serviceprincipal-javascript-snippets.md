---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 817e2ac20f241618d321f0587670835f59726798
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558819"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/claimsMappingPolicies')
    .version('beta')
    .get();

```