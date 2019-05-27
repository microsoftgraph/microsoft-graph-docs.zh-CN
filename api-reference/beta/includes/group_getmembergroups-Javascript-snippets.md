---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 365bbe4f3540f4b46a96d605d3fbb1bf34853276
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444809"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: false
};

let res = await client.api('/groups/{id}/getMemberGroups')
    .version('beta')
    .post(String);

```