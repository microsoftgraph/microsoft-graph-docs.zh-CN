---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7660ca83e486c1fe40456ab270cc60fc348d469b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const call = {
  '@odata.type': '#microsoft.graph.call',
  callbackUri: 'https://bot.contoso.com/callback',
  targets: [
    {
      '@odata.type': '#microsoft.graph.invitationParticipantInfo',
      identity: {
        '@odata.type': '#microsoft.graph.identitySet',
        user: {
          '@odata.type': '#microsoft.graph.identity',
          displayName: 'John',
          id: '112f7296-5fa4-42ca-bae8-6a692b15d4b8'
        }
      }
    }
  ],
  requestedModalities: [
    'audio'
  ],
  mediaConfig: {
    '@odata.type': '#microsoft.graph.serviceHostedMediaConfig'
  }
};

await client.api('/communications/calls')
    .version('beta')
    .post(call);

```