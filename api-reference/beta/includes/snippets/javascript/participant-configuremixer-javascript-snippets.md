---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1167a6e089ccb37ff261b57deacf703d722c3d32
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933838"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const participant = {
  clientContext: "d45324c1-fcb5-430a-902c-f20af696537c",
  participantMixerLevels: [
    {
      participant: "550fae72-d251-43ec-868c-373732c2704f",
      exclusive: true,
      ducking: {
        rampActive: 50,
        rampInactive: 50,
        lowerLevel: 10,
        upperLevel: 50
      },
      sourceLevels: [
        {
          participant: "632899f8-2ea1-4604-8413-27bd2892079f",
          level: 50,
          duckOthers: false
        }
      ]
    }
  ]
};

let res = await client.api('/app/calls/{id}/participants/configureMixer')
    .version('beta')
    .post({participant : participant});

```