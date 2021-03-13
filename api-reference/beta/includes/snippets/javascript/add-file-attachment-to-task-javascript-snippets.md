---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8c7c59570bcd606afffc5fbe04e02f1204e5947
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793742"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    '@odata.type': '#microsoft.graph.fileAttachment',
    name: 'menu.txt',
    contentBytes: 'bWFjIGFuZCBjaGVlc2UgdG9kYXk='
};

await client.api('/me/outlook/tasks/AAMkADAAAANXbdnAAA=/attachments')
    .version('beta')
    .post(attachment);

```