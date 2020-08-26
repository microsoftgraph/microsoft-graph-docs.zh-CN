---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f378f286c35c867d63000e71f2e44e6a0bb51b91
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873925"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/search(q='Contoso Project')')
    .get();

```