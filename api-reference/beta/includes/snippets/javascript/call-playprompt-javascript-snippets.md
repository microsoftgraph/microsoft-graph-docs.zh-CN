---
description: 自动生成的文件。 不修改
ms.openlocfilehash: de3a18d367cb0b02b70a43ef338abc34acc0e076
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36174699"
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
      },
    },
  ],
  loop: false
};

let res = await client.api('/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt')
    .version('beta')
    .post(playPromptOperation);

```