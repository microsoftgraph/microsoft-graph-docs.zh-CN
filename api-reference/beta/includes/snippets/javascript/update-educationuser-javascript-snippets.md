---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 957264892171bd9bebd2562912f88857febe9548
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636510"
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
    .update(educationUser);

```