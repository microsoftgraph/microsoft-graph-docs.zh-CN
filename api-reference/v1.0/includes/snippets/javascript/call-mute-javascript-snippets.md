---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f91557fc0b2a70154ffd667b2758e80458b43807
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/mute')
    .post(muteParticipantOperation);

```