---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62c76a7b8bd5449a5062347e0b65dc0036c4ded00758228a448ed23a0c5a9a08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158558"
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