---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c2c5d415eeb36a72056f08b408f5380d2c878492
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479959"
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