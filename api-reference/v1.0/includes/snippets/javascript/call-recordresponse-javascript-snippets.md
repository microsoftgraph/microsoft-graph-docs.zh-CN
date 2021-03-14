---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7baabdbd0080852fb843384d351e6b49514e7a1f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const recordOperation = {
  bargeInAllowed: true,
  clientContext: 'd45324c1-fcb5-430a-902c-f20af696537c',
  prompts: [
    {
      '@odata.type': '#microsoft.graph.mediaPrompt',
      mediaInfo: {
        uri: 'https://cdn.contoso.com/beep.wav',
        resourceId: '1D6DE2D4-CD51-4309-8DAA-70768651088E'
      }
    }
  ],
  maxRecordDurationInSeconds: 10,
  initialSilenceTimeoutInSeconds: 5,
  maxSilenceTimeoutInSeconds: 2,
  playBeep: true,
  stopTones: [ '#', '1', '*' ]
};

await client.api('/communications/calls/{id}/recordResponse')
    .post(recordOperation);

```