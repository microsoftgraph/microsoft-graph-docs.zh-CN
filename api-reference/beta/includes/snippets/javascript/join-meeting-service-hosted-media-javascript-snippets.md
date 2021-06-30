---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c891ad5f43e1fa5549d7708a343bbd9340481635
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211966"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const call = {
  '@odata.type': '#microsoft.graph.call',
  callbackUri: 'https://bot.contoso.com/callback',
  requestedModalities: [
    'audio'
  ],
  mediaConfig: {
    '@odata.type': '#microsoft.graph.serviceHostedMediaConfig',
    preFetchMedia: [
     {
       uri: 'https://cdn.contoso.com/beep.wav',
       resourceId: 'f8971b04-b53e-418c-9222-c82ce681a582'
     },
     {
       uri: 'https://cdn.contoso.com/cool.wav',
       resourceId: '86dc814b-c172-4428-9112-60f8ecae1edb'
     }
    ],
  },
  chatInfo: {
    '@odata.type': '#microsoft.graph.chatInfo',
    threadId: '19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2',
    messageId: '0'
  },
  meetingInfo: {
    '@odata.type': '#microsoft.graph.organizerMeetingInfo',
    organizer: {
      '@odata.type': '#microsoft.graph.identitySet',
      user: {
        '@odata.type': '#microsoft.graph.identity',
        id: '5810cede-f3cc-42eb-b2c1-e9bd5d53ec96',
        tenantId: 'aa67bd4c-8475-432d-bd41-39f255720e0a',
        displayName: 'Bob'
      }
    },
    allowConversationWithoutHost: true
  },
  tenantId: '86dc81db-c112-4228-9222-63f3esaa1edb'
};

await client.api('/communications/calls')
    .version('beta')
    .post(call);

```