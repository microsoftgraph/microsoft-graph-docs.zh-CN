---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8e5fbe9bb42988962981337f9db73cdcf208267c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478591"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.fileAttachment",
  name: "smile",
  contentBytes: "a0b1c76de9f7="
};

let res = await client.api('/me/messages/AAMkpsDRVK/attachments')
    .version('beta')
    .post({attachment : attachment});

```