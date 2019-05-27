---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef9ab4ba0ea9798beeb0e31d9ab0853dc89885c2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480580"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: "focused",
  senderEmailAddress: {
    name: "Samantha Booth",
    address: "samanthab@adatum.onmicrosoft.com"
  }
};

let res = await client.api('/me/inferenceClassification/overrides')
    .version('beta')
    .post({inferenceClassificationOverride : inferenceClassificationOverride});

```