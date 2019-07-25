---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8a416406a07f4f3c7970799aad90c92c4d006e4d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725331"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/servicePrincipals/{id}/getMemberGroups')
    .version('beta')
    .post(String);

```