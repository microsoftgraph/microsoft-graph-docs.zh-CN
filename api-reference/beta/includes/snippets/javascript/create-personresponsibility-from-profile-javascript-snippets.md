---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22b3210a22889fe60f333ad9c2c287760fdf4140
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  description: 'Member of the Microsoft API Council',
  displayName: 'API Council',
  collaborationTags: [
    'askMeAbout'
  ]
};

await client.api('/me/responsibilities')
    .version('beta')
    .post(string);

```