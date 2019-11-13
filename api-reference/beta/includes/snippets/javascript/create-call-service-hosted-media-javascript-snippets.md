---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0a3cff4895f8e2e3f4e874e9a8a264c277b91aa
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const call = {
  @odata.type: "#microsoft.graph.call",
  callbackUri: "https://bot.contoso.com/callback",
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
    @odata.type: "#microsoft.graph.serviceHostedMediaConfig",
  }
};

let res = await client.api('/communications/calls')
    .version('beta')
    .post(call);

```