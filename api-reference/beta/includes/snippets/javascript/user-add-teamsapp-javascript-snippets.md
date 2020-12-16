---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbc9d93a90bab144f3e9a01a574f4e4fed47c855
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userScopeTeamsAppInstallation = {
   teamsApp@odata.bind:"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
};

let res = await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps')
    .version('beta')
    .post(userScopeTeamsAppInstallation);

```