---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f0cf0b10b1193748de4d3eface1a37b991719250
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467046"
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