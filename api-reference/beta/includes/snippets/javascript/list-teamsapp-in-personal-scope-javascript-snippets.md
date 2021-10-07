---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11f47738137c0592622ddce457e40158bc2d229c78be294a157575ba8f1a5118
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215720"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('appDefinitions/any(a:a/allowedInstallationScopes has \'personal\')')
    .expand('appDefinitions($select=id,displayName,allowedInstallationScopes)')
    .get();

```