---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45af250478353824e1e7fd1f8999f12816fa5ec9
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps')
    .version('beta')
    .filter('teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'')
    .expand('teamsAppDefinition')
    .get();

```