---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e66a9672bbe19f45f66da263162ba2029673809
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/contacts/{id}/getMemberGroups')
    .version('beta')
    .post(String);

```