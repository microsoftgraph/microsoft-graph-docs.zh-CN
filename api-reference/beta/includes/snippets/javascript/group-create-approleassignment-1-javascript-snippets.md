---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01a04df45058963d54b151d6713054d305b0ddab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946051"
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