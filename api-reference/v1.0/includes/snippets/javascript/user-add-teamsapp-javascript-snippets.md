---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a25ad102348e2e706719316a83e61095b3699f93
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userScopeTeamsAppInstallation = {
   teamsApp@odata.bind:"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
};

let res = await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps')
    .post(userScopeTeamsAppInstallation);

```