---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa6c9f348e4a33c48235d9f9043e7bd45e5c3c8a
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765960"
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