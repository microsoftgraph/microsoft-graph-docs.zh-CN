---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2efcbf125863b0e5120bf22048cfd8a7d2b327ee
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444158"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: "destinationId-value"
};

let res = await client.api('/me/mailFolders/{id}/move')
    .version('beta')
    .post(mailFolder);

```