---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 963662a959ef37341b6333e8c992d7f2ff8a79ad
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437207"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/me/getMemberGroups')
    .version('beta')
    .post(String);

```