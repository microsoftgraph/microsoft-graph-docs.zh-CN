---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9c9570a6125eeabc8d17eca5578ef81617233e5c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478956"
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