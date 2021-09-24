---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88bd102f7962580e4ca01b8ac9cd8284c8603654
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const startHoldMusicOperation = {
  customPrompt: {
    '@odata.type': '#microsoft.graph.mediaPrompt',
    mediaInfo: {
      '@odata.type': '#microsoft.graph.mediaInfo',
      uri: 'https://bot.contoso.com/onHold.wav',
    },
  },
  clientContext: 'd45324c1-fcb5-430a-902c-f20af696537c',
};

await client.api('/communications/calls/e141b67c-90fd-455d-858b-b48a40b9cc8d/participants/fa1e9582-7145-4ca3-bcd8-577f561fcb6e/startHoldMusic')
    .version('beta')
    .post(startHoldMusicOperation);

```