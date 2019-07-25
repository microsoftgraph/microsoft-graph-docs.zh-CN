---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 94a30a8922fc4ddce3d7eb44078ae87f18914c3d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732315"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  receivedDateTime: "datetime-value",
  sentDateTime: "datetime-value",
  hasAttachments: true,
  subject: "subject-value",
  body: {
    contentType: "",
    content: "content-value"
  },
  bodyPreview: "bodyPreview-value"
};

let res = await client.api('/me/mailFolders/{id}/messages')
    .post({message : message});

```