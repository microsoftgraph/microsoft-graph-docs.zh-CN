---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac8aaa469099c2aceb3fe69131e7bd0be954f1b5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956013"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroupMember = {
  '@odata.type': '#microsoft.graph.externalGroupMember',
  id: 'e5477431-1038-484e-bf69-1dfedb97a110',
  type: 'group',
  identitySource: 'azureActiveDirectory'
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .version('beta')
    .post(externalGroupMember);

```