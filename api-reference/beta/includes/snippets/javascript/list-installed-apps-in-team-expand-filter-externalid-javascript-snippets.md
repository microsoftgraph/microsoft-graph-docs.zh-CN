---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 350c872b028a541f15981abf9f61f6354d166578
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps')
    .version('beta')
    .filter('teamsApp/externalId eq \'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee\'')
    .expand('teamsApp,teamsAppDefinition')
    .get();

```