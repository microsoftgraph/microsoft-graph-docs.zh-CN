---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b4e13e65d92d1bbabc8ebb3e3ee98800759de107f33038775b23b2502a0474a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215936"
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