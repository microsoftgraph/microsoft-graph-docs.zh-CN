---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe33671fbad3fe6432a8fc08a430664f403e98fe
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const playPromptOperation = {
  clientContext: "d45324c1-fcb5-430a-902c-f20af696537c",
  prompts: [
    {
      @odata.type: "#microsoft.graph.mediaPrompt",
      mediaInfo: {
        @odata.type: "#microsoft.graph.mediaInfo",
        uri: "https://cdn.contoso.com/beep.wav",
        resourceId: "1D6DE2D4-CD51-4309-8DAA-70768651088E"
      }
    }
  ]
};

let res = await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt')
    .post(playPromptOperation);

```