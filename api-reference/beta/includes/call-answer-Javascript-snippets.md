---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2079cd1d22cef1632c0d008ca858229c4ae43f22
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456348"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const answer = {
  callbackUri: "callbackUri-value",
  mediaConfig: {
    @odata.type: "#microsoft.graph.appHostedMediaConfig",
    blob: "<media config blob>"
  },
  acceptedModalities: [
    "audio"
  ]
};

let res = await client.api('/app/calls/{id}/answer')
    .version('beta')
    .post(answer);

```