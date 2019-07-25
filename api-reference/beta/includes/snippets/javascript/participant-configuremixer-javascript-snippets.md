---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f9fe7f70e50e18512199e1fd9110de4a31bb462a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730590"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
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
    .post(CommsOperation);

```