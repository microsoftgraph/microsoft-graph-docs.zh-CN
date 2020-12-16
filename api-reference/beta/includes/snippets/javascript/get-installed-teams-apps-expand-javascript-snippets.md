---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72ff0db04738db85bd04e0e80a1bb877547131e8
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/installedApps/{id}')
    .version('beta')
    .expand('teamsAppDefinition')
    .get();

```