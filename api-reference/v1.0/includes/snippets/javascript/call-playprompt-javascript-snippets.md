---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86881e7744cae6c1739d163e0dbf7fe43a76f1a4d73c7e80ea6869027cd1d460
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279696"
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
      }
    }
  ]
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/playPrompt')
    .post(playPromptOperation);

```