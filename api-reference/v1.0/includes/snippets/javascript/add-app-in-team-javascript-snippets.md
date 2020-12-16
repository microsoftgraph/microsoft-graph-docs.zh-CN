---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b95e59e596f7a8f81aa719eb7fe92a033e652608
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppInstallation = {
   teamsApp@odata.bind:"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
};

let res = await client.api('/teams/87654321-0abc-zqf0-321456789q/installedApps')
    .post(teamsAppInstallation);

```