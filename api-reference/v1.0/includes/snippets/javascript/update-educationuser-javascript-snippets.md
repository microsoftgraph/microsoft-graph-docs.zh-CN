---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ea3328ced27cb1322b510f310ea7619d9931a810
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732682"
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

let res = await client.api('/education/users/{user-id}')
    .update({educationUser : educationUser});

```