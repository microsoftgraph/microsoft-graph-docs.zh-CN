---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a9dff7de0c5a3346602ac53a58b41ee26692ceb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const recordOperation = {
  bargeInAllowed: true,
  clientContext: "d45324c1-fcb5-430a-902c-f20af696537c",
  prompts: [
    {
      @odata.type: "#microsoft.graph.mediaPrompt",
      mediaInfo: {
        uri: "https://cdn.contoso.com/beep.wav",
        resourceId: "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      }
    }
  ],
  maxRecordDurationInSeconds: 10,
  initialSilenceTimeoutInSeconds: 5,
  maxSilenceTimeoutInSeconds: 2,
  playBeep: true,
  stopTones: [ "#", "1", "*" ]
};

let res = await client.api('/communications/calls/{id}/recordResponse')
    .post(recordOperation);

```