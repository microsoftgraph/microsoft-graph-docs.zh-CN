---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 195be5614c6a364c4b2d474280847d70b7f491c0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: "destinationId-value"
};

let res = await client.api('/me/mailFolders/{id}/copy')
    .version('beta')
    .post(mailFolder);

```