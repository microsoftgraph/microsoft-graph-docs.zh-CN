---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e5a15831f34c016c4ec026e6c71cfbac5f29c4a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalGroupMember = {
  id: '1431b9c38ee647f6a',
  type: 'externalGroup',
};

await client.api('/external/connections/contosohr/groups/31bea3d537902000/members')
    .version('beta')
    .post(externalGroupMember);

```