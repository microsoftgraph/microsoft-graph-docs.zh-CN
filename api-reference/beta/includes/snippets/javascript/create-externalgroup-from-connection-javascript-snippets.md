---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2dad80ba80518d9f2d0e9c122b3da23fb08ca16
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroup = {
  id: '31bea3d537902000',
  displayName: 'Contoso Marketing',
  description: 'The product marketing team'
};

await client.api('/external/connections/contosohr/groups')
    .version('beta')
    .post(externalGroup);

```