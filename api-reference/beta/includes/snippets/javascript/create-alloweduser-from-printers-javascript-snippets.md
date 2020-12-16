---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e17417db29d93cbf2bb2c8a04dbf42e43159086
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  @odata.id: "https://graph.microsoft.com/beta/users/{id}"
};

let res = await client.api('/print/shares/{id}/allowedUsers/$ref')
    .version('beta')
    .post(user);

```