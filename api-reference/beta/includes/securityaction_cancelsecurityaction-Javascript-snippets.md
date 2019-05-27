---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 870a83db65e5f5b4fb1f92660bf227d347c4cc65
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453262"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/securityActions/{id}/cancelSecurityAction')
    .version('beta')
    .post();

```