---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d0ccd148caf7f07964fbe4cad2bf22dc4978f8d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804814"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const playPromptOperation = {
  clientContext: 'd45324c1-fcb5-430a-902c-f20af696537c',
  prompts: [
    {
      '@odata.type': '#microsoft.graph.mediaPrompt',
      mediaInfo: {
        '@odata.type': '#microsoft.graph.mediaInfo',
        uri: 'https://cdn.contoso.com/beep.wav',
        resourceId: '1D6DE2D4-CD51-4309-8DAA-70768651088E'
      },
    },
  ],
  loop: false
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt')
    .version('beta')
    .post(playPromptOperation);

```