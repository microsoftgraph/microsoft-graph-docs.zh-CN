---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 88e147d600315f26ee826e72a30932f3a2535b0e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520122"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  subject: "subject-value",
  body: {
    contentType: "",
    content: "content-value"
  },
  inferenceClassification: "other"
};

let res = await client.api('/me/messages/{id}')
    .version('beta')
    .update({message : message});

```