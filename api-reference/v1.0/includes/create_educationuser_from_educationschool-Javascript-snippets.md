---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8642aafe1d11c8701907706e0376794c4da83f25
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440448"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/v1.0/education/users/14008"
};

let res = await client.api('/education/schools/{id}/users/$ref')
    .post({educationUser : educationUser});

```