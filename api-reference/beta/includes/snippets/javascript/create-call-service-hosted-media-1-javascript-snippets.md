---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c893afa4088aa2b275acf689b47603cdb6f614b5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220261"
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
  callOptions: {
    '@odata.type': '#microsoft.graph.outgoingCallOptions',
    isContentSharingNotificationEnabled: true
  },
  mediaConfig: {
    '@odata.type': '#microsoft.graph.serviceHostedMediaConfig'
  }
};

await client.api('/communications/calls')
    .version('beta')
    .post(call);

```