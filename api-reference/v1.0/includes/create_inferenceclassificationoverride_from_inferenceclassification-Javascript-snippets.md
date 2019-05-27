---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f0cf0b10b1193748de4d3eface1a37b991719250
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468638"
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
    .post({inferenceClassificationOverride : inferenceClassificationOverride});

```