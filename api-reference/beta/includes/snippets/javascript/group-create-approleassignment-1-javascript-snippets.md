---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 418d0920050a2662488a72a85a4810926cb418eaa50d3f942678274af96c19c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = {
  principalId: '7679d9a4-2323-44cd-b5c2-673ec88d8b12',
  resourceId: '076e8b57-bac8-49d7-9396-e3449b685055',
  appRoleId: '00000000-0000-0000-0000-000000000000'
};

await client.api('/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments')
    .version('beta')
    .post(appRoleAssignment);

```