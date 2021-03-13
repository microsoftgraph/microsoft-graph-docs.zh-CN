---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a4cc83030045cb997e185985b4d1de9f606b4c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785216"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroup = {
  '@odata.type': '#microsoft.graph.externalGroup',
  id: '31bea3d537902000',
  displayName: 'Contoso Marketing',
  description: 'The product marketing team'
};

await client.api('/external/connections/contosohr/groups')
    .version('beta')
    .post(externalGroup);

```