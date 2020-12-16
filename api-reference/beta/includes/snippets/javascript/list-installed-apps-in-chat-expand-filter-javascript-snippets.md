---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25f43c3e6faa94ab9814ff8f8b0ed92beefc6957
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps')
    .version('beta')
    .filter('teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'')
    .expand('teamsAppDefinition')
    .get();

```