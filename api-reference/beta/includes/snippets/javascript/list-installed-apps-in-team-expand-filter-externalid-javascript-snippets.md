---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25f4e490512772e0196599e916a77a54ef435b9d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps')
    .version('beta')
    .filter('teamsApp/externalId eq \'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee\'')
    .expand('teamsAppDefinition')
    .get();

```