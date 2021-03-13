---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a47e2cbded70cad8acbe731ccb4418c8fcd0e562
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806518"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const answer = {
  callbackUri: 'https://bot.contoso.com/api/calls',
  acceptedModalities: [ 'audio' ],
  mediaConfig: {
    '@odata.type': '#microsoft.graph.appHostedMediaConfig',
    blob: '<Media Session Configuration Blob>'
  }
};

await client.api('/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer')
    .version('beta')
    .post(answer);

```