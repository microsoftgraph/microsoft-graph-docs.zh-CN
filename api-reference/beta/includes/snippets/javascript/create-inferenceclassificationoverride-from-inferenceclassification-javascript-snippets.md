---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c2de100bddeee8cd1a4f5194150ef089eb2a2c2
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636485"
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
    .post(inferenceClassificationOverride);

```