---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57548a1a5fb4176ecbe2c93d599e1b63abdc3e77
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const answer = {
  callbackUri: 'callbackUri-value',
  mediaConfig: {
    '@odata.type': '#microsoft.graph.appHostedMediaConfig',
    blob: '<Media Session Configuration Blob>'
  },
  acceptedModalities: [
    'audio'
  ],
  participantCapacity: 200
};

await client.api('/communications/calls/{id}/answer')
    .version('beta')
    .post(answer);

```