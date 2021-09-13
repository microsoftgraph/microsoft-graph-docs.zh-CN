---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74842aaef2fedf2cb9431cafe95d6ff07845b735a654dad66074e6fe559c6dd4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161976"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsAppInstallation = {
   'teamsApp@odata.bind':'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a'
};

await client.api('/teams/87654321-0abc-zqf0-321456789q/installedApps')
    .post(teamsAppInstallation);

```