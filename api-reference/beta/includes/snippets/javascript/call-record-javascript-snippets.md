---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e9093fd8f1b77dfd2c292918c4292c98f2943ff
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933821"
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
  stopTones: [ "#", "11", "*" ]
};

let res = await client.api('/app/calls/{id}/record')
    .version('beta')
    .post(recordOperation);

```