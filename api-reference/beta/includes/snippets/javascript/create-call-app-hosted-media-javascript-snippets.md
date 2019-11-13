---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 772fd09abfd488849d853f0ca4df216c391bb6a8
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302125"
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
      application: {
        @odata.type: "#microsoft.graph.identity",
        displayName: "Calling Bot",
        id: "2891555a-92ff-42e6-80fa-6e1300c6b5c6"
      }
    },
    region: null,
    languageId: null
  },
  targets: [
    {
      @odata.type: "#microsoft.graph.participantInfo",
      identity: {
        @odata.type: "#microsoft.graph.identitySet",
        user: {
          @odata.type: "#microsoft.graph.identity",
          displayName: "John",
          id: "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
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