---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 222fb1af940c6505d1ae7aa1865b2b6100632be0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710160"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const applicationServicePrincipal = {
  displayName: "My custom name"
};

let res = await client.api('/applicationTemplates/{id}/instantiate')
    .version('beta')
    .post(applicationServicePrincipal);

```