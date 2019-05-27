---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 903796230c79bd412100af396bedae71175cd132
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  @odata.id:"https://graph.microsoft.com/beta/education/users/14008"
};

let res = await client.api('/education/schools/'id'/users/$ref')
    .version('beta')
    .post({educationUser : educationUser});

```