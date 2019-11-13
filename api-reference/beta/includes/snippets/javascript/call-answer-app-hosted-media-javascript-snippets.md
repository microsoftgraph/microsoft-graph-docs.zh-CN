---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3e265e13f5404ecca1ff89f58ff59634a41cd24
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302352"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const answer = {
  callbackUri: "https://bot.contoso.com/api/calls",
  acceptedModalities: [ "audio" ],
  mediaConfig: {
    @odata.type: "#microsoft.graph.appHostedMediaConfig",
    blob: "<Media Session Configuration Blob>"
  }
};

let res = await client.api('/communications/calls/57DAB8B1894C409AB240BD8BEAE78896/answer')
    .version('beta')
    .post(answer);

```