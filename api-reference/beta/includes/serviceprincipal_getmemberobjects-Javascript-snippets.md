---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f85dc129f6bec87bdb77a7b41a89c05a59c156c4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453255"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/servicePrincipals/{id}/getMemberObjects')
    .version('beta')
    .post(String);

```