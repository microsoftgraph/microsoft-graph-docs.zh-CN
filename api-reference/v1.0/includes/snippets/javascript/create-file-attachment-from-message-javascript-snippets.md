---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a41edfdec3e0c5234a3e87a4e3c00a88211a1fdd
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.fileAttachment",
  name: "smile",
  contentBytes: "base64R0lGODdhEAYEAA7"
};

let res = await client.api('/me/messages/AAMkpsDRVK/attachments')
    .post({attachment : attachment});

```