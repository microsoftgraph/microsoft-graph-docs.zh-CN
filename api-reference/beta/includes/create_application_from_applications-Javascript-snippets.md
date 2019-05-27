---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9c9570a6125eeabc8d17eca5578ef81617233e5c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  allowPublicClient: true,
  displayName: "Display name"
};

let res = await client.api('/applications')
    .version('beta')
    .post({application : application});

```