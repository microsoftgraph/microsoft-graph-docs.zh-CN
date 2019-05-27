---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a604165b281286aa8e1f16bfd4a2b314e58f54ea
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders')
    .get();

```