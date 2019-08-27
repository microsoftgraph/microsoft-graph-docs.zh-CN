---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8b764fa4c9f24b8bfb0973815cdb8b581c3beb75
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636726"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  receivedDateTime: "2016-10-19T10:37:00Z",
  sentDateTime: "2016-10-19T10:37:00Z",
  hasAttachments: true,
  subject: "subject-value",
  body: {
    contentType: "",
    content: "content-value"
  },
  bodyPreview: "bodyPreview-value"
};

let res = await client.api('/me/mailFolders/{id}/messages')
    .version('beta')
    .post(message);

```