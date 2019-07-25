---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b981006aa71d7bd70cc6740553657f78fea81528
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    @odata.type: "#microsoft.graph.fileAttachment",
    name: "menu.txt",
    contentBytes: "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk="   
};

let res = await client.api('/me/events/AAMkAGI1AAAt9AHjAAA=/attachments')
    .post({attachment : attachment});

```