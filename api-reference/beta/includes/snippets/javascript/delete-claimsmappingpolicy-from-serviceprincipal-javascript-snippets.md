---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f93c9b3af7315221c364d0b21b24f4fa2f00e025
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref')
    .version('beta')
    .delete();

```