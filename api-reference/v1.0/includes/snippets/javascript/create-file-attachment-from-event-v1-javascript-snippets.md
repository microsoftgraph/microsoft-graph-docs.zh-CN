---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a15e40af5b74310a7bda8b32a882cc6bca1e1cd491d3136b5342f0225e59c48e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332608"
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