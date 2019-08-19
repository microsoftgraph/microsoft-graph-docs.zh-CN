---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f27f06d0cb79674396f2c3c2ac2da53aa081c40b
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460915"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    @odata.type: "#microsoft.graph.fileAttachment",
    name: "menu.txt",
    contentBytes: "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
};

let res = await client.api('/me/events('AAMkAGI1AAAt9AHjAAA=')/attachments')
    .version('beta')
    .post({attachment : attachment});

```