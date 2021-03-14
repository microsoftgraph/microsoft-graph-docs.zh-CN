---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 029b58a484a308ef8bd0c6463462d43676781c2b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802114"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userScopeTeamsAppInstallation = {
   'teamsApp@odata.bind':'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a'
};

await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps')
    .post(userScopeTeamsAppInstallation);

```