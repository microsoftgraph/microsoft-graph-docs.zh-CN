---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 94a30a8922fc4ddce3d7eb44078ae87f18914c3d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460451"
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