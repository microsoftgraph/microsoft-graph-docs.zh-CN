---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efbef8529d862d29b474e496c851648775e37c20
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274715"
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
    .post(call);

```