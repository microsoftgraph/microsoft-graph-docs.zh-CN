---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 299673f5a65b09a85c6ed6a90cdb918271dda7c61318a3d5a5b5e8fbaf1e13e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userScopeTeamsAppInstallation = await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk')
    .get();

```