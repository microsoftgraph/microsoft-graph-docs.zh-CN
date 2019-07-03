---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a9cabbb691937913431eaf67ab7b8a4044be7219
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467937"
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
    .update({message : message});

```