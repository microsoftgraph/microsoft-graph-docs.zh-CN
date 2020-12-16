---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f50fa9b0f680eb5c93af9f4da72006d76fbd968
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689317"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'')
    .get();

```