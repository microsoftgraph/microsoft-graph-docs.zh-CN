---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0717fa1d3fb1281afabe670bc890a509e1338d5
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('distributionMethod eq 'organization'')
    .get();

```