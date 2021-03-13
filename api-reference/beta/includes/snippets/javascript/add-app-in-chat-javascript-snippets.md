---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f2db578d60f776dbbe07c7e595db8922d312bca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775687"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppInstallation = {
'teamsApp@odata.bind':'https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a'
};

await client.api('/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps')
    .version('beta')
    .post(teamsAppInstallation);

```