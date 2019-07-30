---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1bc09ea0cca8472729bf5a8ae09e4e332351f10f
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932359"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppInstallation = {
   teamsApp@odata.bind:"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
};

let res = await client.api('/teams/{id}/installedApps')
    .post({teamsAppInstallation : teamsAppInstallation});

```