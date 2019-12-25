---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0063f9235ff004ffa111d4fa00ca17f79b7a2952
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865800"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const muteParticipantOperation = {
  clientContext: "d45324c1-fcb5-430a-902c-f20af696537c"
};

let res = await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/participants/2765eb15-01f8-47c6-b12b-c32111a4a86f/mute')
    .post(muteParticipantOperation);

```