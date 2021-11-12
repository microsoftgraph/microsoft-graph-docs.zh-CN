---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9218b9c9c525bd85f2fea9bbeb8883c5f9947c7bab05fb27e44f85f0998aab3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106640"
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

await client.api('/me/messages/AAMkAGE1M88AADUv0uFAAA=/attachments')
    .version('beta')
    .post(attachment);

```