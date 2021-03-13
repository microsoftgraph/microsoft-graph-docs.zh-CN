---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55f2eb2c6ea6dd85206dd2a518cb4a793ef54ad6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personWebsite = {
  description: 'Lyn Damer play in the Women\'s 1st Division (Toppserien) in Norway'
};

await client.api('/me/profile/websites/{id}')
    .version('beta')
    .update(personWebsite);

```