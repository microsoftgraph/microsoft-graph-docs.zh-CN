---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06b9a54cebe1b63f5039f29b75049345c5aa2471
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  displayName: 'Rogelio Cazares',
  givenName: 'Rogelio',
  middleName: 'Fernando',
  surname: 'Cazares',
};

await client.api('/education/users/{user-id}')
    .update(educationUser);

```