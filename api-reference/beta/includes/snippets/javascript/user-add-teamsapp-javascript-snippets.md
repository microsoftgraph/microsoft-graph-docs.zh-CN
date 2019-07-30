---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d29b5fc04349817d17a4051118c621e256acd28a
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931445"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppInstallation = {
   teamsApp@odata.bind:"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
};

let res = await client.api('/users/{id}/teamwork/installedApps')
    .version('beta')
    .post({teamsAppInstallation : teamsAppInstallation});

```