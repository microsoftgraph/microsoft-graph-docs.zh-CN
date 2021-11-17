---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 093041542c6b915987d802ce651ec2a16fc918e273c6840769937d853900f9d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219538"
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