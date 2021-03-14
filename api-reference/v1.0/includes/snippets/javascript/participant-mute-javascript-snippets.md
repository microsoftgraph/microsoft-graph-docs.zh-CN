---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d7a0305950ec7531398f37d9f43abbd9755bd22
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantOperation = {
  clientContext: 'd45324c1-fcb5-430a-902c-f20af696537c'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants/2765eb15-01f8-47c6-b12b-c32111a4a86f/mute')
    .post(muteParticipantOperation);

```