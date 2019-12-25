---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e538e8205e92ea79cb9737ee8f6b307e3d539215
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871128"
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
    .post(answer);

```