---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7c00fd37a8b9f1b373d5476c5da24152b995b50
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41119702"
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

let res = await client.api('/me/outlook/tasks/AAMkADAAAANXbdnAAA=/attachments')
    .version('beta')
    .post(attachment);

```