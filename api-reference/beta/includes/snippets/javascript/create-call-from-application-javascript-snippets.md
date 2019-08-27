---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 48fae86f0a890d63eb163ae9057d4e1bfd5503a0
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636590"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const call = {
  callbackUri: "https://bot.contoso.com/api/calls",
  mediaConfig: {
    @odata.type: "#microsoft.graph.serviceHostedMediaConfig",
    preFetchMedia: [
      {
        uri: "https://cdn.contoso.com/beep.wav",
        resourceId: "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      },
      {
        uri: "https://cdn.contoso.com/cool.wav",
        resourceId: "1D6DE2D4-CD51-4309-8DAA-70768651088F"
      }
    ]
  },
  source: {
    identity: {
      application: {
        id: "8A34A46B-3D17-4ADC-8DCE-DC4E7D572698"
      }
    },
    languageId: "languageId-value",
    region: "region-value"
  },
  subject: "Test Call",
  targets: [
    {
      identity: {
        user: {
          id: "550fae72-d251-43ec-868c-373732c2704f",
          tenantId: "72f988bf-86f1-41af-91ab-2d7cd011db47",
          displayName: "Heidi Steen"
        }
      }
    }
  ],
  tenantId: "tenantId-value"
};

let res = await client.api('/app/calls')
    .version('beta')
    .post(call);

```