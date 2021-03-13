---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daa824da515418f87ee9e83377c208fe04927bbd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798931"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const call = {
  '@odata.type': '#microsoft.graph.call',
  callbackUri: 'https://bot.contoso.com/callback',
  source: {
    '@odata.type': '#microsoft.graph.participantInfo',
    identity: {
      '@odata.type': '#microsoft.graph.identitySet',
      application: {
        '@odata.type': '#microsoft.graph.identity',
        displayName: 'Calling Bot',
        id: '2891555a-92ff-42e6-80fa-6e1300c6b5c6'
      }
    },
    region: null,
    languageId: null
  },
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
    '@odata.type': '#microsoft.graph.appHostedMediaConfig',
    blob: '<Media Session Configuration>'
  }
};

await client.api('/communications/calls')
    .version('beta')
    .post(call);

```