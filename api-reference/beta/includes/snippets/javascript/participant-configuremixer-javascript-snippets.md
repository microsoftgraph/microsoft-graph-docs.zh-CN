---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e64d2564b96eaf42a4190f0fc671ff25263e6231
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302817"
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

let res = await client.api('/communications/calls/{id}/participants/configureMixer')
    .version('beta')
    .post(participant);

```