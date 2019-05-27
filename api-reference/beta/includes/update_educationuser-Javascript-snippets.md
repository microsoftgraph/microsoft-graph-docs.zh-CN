---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c2c5d415eeb36a72056f08b408f5380d2c878492
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  displayName: "Rogelio Cazares",
  givenName: "Rogelio",
  middleName: "Fernando",
  surname: "Cazares",
};

let res = await client.api('/education/users/13020')
    .version('beta')
    .update({educationUser : educationUser});

```