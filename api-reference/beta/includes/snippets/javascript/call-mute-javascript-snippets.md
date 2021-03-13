---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab3cc2434f51a4224a9e399311a1b1bf06376f60
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804047"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantOperation = {
  clientContext: 'clientContext-value'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/mute')
    .version('beta')
    .post(muteParticipantOperation);

```