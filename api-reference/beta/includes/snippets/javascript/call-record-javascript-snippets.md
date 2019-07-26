---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 09211347bc6e316be50410c81433394be2b93406
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  bargeInAllowed: true,
  clientContext: "d45324c1-fcb5-430a-902c-f20af696537c",
  prompts: [
    {
      @odata.type: "#microsoft.graph.mediaPrompt",
      mediaInfo: {
        uri: "https://cdn.contoso.com/beep.wav",
        resourceId: "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      loop: 5
    }
  ],
  maxRecordDurationInSeconds: 1800,
  initialSilenceTimeoutInSeconds: 10,
  maxSilenceTimeoutInSeconds: 2,
  recordingFormat: "wav",
  playBeep: true,
  streamWhileRecording: true,
  stopTones: [ "#", "11", "*" ]
};

let res = await client.api('/app/calls/{id}/record')
    .version('beta')
    .post(CommsOperation);

```