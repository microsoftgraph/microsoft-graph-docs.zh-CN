---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f127c40a2a47385d03cd1d031b4c6961ed65ce72
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636613"
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
    .post(teamsAppInstallation);

```