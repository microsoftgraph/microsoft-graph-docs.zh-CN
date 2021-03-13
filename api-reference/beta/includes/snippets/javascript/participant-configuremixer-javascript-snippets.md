---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68011fc791dfe3664574f448f3648a1eca739cd9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785482"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const participant = {
  clientContext: 'd45324c1-fcb5-430a-902c-f20af696537c',
  participantMixerLevels: [
    {
      participant: '550fae72-d251-43ec-868c-373732c2704f',
      exclusive: true,
      ducking: {
        rampActive: 50,
        rampInactive: 50,
        lowerLevel: 10,
        upperLevel: 50
      },
      sourceLevels: [
        {
          participant: '632899f8-2ea1-4604-8413-27bd2892079f',
          level: 50,
          duckOthers: false
        }
      ]
    }
  ]
};

await client.api('/communications/calls/{id}/participants/configureMixer')
    .version('beta')
    .post(participant);

```