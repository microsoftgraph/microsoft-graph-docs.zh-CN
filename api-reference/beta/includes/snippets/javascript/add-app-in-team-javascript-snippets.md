---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f9ab3392cf543f184b6f9619d1aa7bf6bee92f2c6477ff38aa53a3cb35dc5a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105510"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppInstallation = {
   'teamsApp@odata.bind':'https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a'
};

await client.api('/teams/87654321-0abc-zqf0-321456789q/installedApps')
    .version('beta')
    .post(teamsAppInstallation);

```