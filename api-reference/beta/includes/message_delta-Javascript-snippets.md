---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2c1d2532f1f545d85dfd5720959aa8a07425a297
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444039"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}/messages/delta')
    .version('beta')
    .get();

```