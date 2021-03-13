---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d464d9a6c0f79f6b61e8c44d2cdd91e81420aa28
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    '@odata.type': '#microsoft.graph.referenceAttachment',
    name: 'Personal pictures',
    sourceUrl: 'https://contoso.com/personal/mario_contoso_net/Documents/Pics',
    providerType: 'oneDriveConsumer',
    permission: 'Edit',
    isFolder: 'True'
};

await client.api('/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments')
    .version('beta')
    .post(attachment);

```