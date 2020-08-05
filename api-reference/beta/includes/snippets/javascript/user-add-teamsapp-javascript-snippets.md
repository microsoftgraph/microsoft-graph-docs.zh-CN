---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb11161bef2a7ac39f13cd7c4eb74b81a977e476
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46569918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userScopeTeamsAppInstallation = {
   teamsApp@odata.bind:"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
};

let res = await client.api('/users/{id}/teamwork/installedApps')
    .version('beta')
    .post(userScopeTeamsAppInstallation);

```