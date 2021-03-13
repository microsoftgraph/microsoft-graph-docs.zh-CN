---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3840e5deb0fe3cac0c1029686e6381c607a4e47
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790843"
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