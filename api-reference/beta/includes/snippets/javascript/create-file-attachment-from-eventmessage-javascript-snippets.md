---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c6e6648284cc49b0e5384a918668055201922c67
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#Microsoft.OutlookServices.FileAttachment",
  name: "name-value",
  contentType: "contentType-value",
  isInline: false,
  contentLocation: "contentLocation-value",
  contentBytes: "contentBytes-value"
};

let res = await client.api('/me/messages/{id}/attachments')
    .version('beta')
    .post({attachment : attachment});

```