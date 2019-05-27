---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 101e6b522909a2c7ab66c53a7149c6487612f55b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446475"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{id}/scopedMembers')
    .version('beta')
    .get();

```