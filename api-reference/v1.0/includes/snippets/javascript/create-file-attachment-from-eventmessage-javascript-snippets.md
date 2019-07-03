---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c634633cce1ec4fea0efa612bf9e292d39579d85
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493099"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "microsoft.graph.fileAttachment",
  name: "name-value",
  contentType: "contentType-value",
  isInline: false,
  contentLocation: "contentLocation-value",
  contentBytes: "base64-contentBytes-value"
};

let res = await client.api('/me/messages/{id}/attachments')
    .post({attachment : attachment});

```