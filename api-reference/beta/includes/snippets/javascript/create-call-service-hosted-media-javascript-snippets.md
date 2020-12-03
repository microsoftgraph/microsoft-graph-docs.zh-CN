---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad5c09a2a7d97205a50eaafa17d2cef1d17e2386
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const call = {
  @odata.type: "#microsoft.graph.call",
  callbackUri: "https://bot.contoso.com/callback",
  source: {
    @odata.type: "#microsoft.graph.participantInfo",
    identity: {
      @odata.type: "#microsoft.graph.identitySet",
      applicationInstance: {
        @odata.type: "#microsoft.graph.identity",
        displayName: "Calling Bot",
        id: "3d913abb-aec0-4964-8fa6-3c6850c4f278"
      },
    },
    countryCode: null,
    endpointType: null,
    region: null,
    languageId: null
  },
  targets: [
    {
      @odata.type: "#microsoft.graph.invitationParticipantInfo",
      identity: {
        @odata.type: "#microsoft.graph.identitySet",
        phone: {
          @odata.type: "#microsoft.graph.identity",
          id: "+12345678901"
        }
      }
    }
  ],
  requestedModalities: [
    "audio"
  ],
  mediaConfig: {
    @odata.type: "#microsoft.graph.appHostedMediaConfig",
    blob: "<Media Session Configuration>"
  }
};

let res = await client.api('/communications/calls')
    .version('beta')
    .post(call);

```