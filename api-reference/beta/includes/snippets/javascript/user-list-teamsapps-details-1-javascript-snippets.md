---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5306161d52b7ea75434e72416317e98048fc917df0c2d855608f608832ad6856
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220744"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userScopeTeamsAppInstallation = await client.api('/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=')
    .version('beta')
    .expand('teamsAppDefinition')
    .get();

```