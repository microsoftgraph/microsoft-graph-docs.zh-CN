---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f53b176676529e1dd09d7b9e3ebe0a233659cc7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097190"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroupMember = {
  id: 'e5477431-1038-484e-bf69-1dfedb97a110',
  type: 'externalGroup',
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .version('beta')
    .post(externalGroupMember);

```