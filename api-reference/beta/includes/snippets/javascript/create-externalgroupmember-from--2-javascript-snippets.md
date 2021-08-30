---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca5c70f5704d1729e7681270530c6c9af145a4480ace5bebc805c3b9d4b518f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroupMember = {
  id: 'e5477431-1038-484e-bf69-1dfedb97a110',
  type: 'group',
  identitySource: 'azureActiveDirectory'
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .version('beta')
    .post(externalGroupMember);

```