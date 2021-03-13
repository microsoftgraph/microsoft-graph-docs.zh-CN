---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 404a285f5cf798957fac7f77fab60079464bd75f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770109"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps')
    .version('beta')
    .filter('teamsApp/externalId eq \'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee\'')
    .expand('teamsAppDefinition')
    .get();

```