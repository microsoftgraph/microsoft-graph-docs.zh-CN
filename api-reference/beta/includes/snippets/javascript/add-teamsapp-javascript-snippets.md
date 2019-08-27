---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 113860a84e07a7c65aeee7536e1933dd6086ae22
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636619"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppInstallation = {
   teamsApp@odata.bind:"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
};

let res = await client.api('/teams/87654321-0abc-zqf0-321456789q/installedApps')
    .version('beta')
    .post(teamsAppInstallation);

```