---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 585119b88506cb321c28a73dd3e9ddd3e377a3b9ec48c03960604059f6b01055
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409366"
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
    .post(answer);

```