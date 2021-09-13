---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec1bd22c177b81447b7102b7b510855d93018024151add1e75bd81fe90aa9ebd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409368"
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
    .post(answer);

```