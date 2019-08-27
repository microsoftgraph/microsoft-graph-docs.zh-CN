---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8d56bcc02a1fd07261437271b2a9c5655bf499c4
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636673"
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
    .update(message);

```