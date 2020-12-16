---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98a02f0ac939771296b1956f642c00eda4f92970
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  @odata.id: "https://graph.microsoft.com/beta/groups/{id}"
};

let res = await client.api('/print/shares/{id}/allowedGroups/$ref')
    .version('beta')
    .post(group);

```