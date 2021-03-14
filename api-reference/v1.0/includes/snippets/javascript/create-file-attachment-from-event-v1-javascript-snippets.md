---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8dcf382e2972293d4c0312cdc8179d1bc927359
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    '@odata.type': '#microsoft.graph.fileAttachment',
    name: 'menu.txt',
    contentBytes: 'base64bWFjIGFuZCBjaGVlc2UgdG9kYXk='   
};

await client.api('/me/events/AAMkAGI1AAAt9AHjAAA=/attachments')
    .post(attachment);

```