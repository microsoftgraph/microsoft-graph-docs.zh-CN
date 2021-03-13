---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2b7d72374ba9077293355dd07b74d32be2cccf6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: 'text',
      content: 'I attached a reference to a file on OneDrive.'
    },
    attachments: [{
      '@odata.type': '#microsoft.graph.referenceAttachment', 
      name: 'Personal pictures', 
      sourceUrl: 'https://contoso.com/personal/mario_contoso_net/Documents/Pics', 
      providerType: 'oneDriveConsumer', 
      permission: 'Edit', 
      isFolder: 'True'
    } ]
  }
};

await client.api('/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply')
    .version('beta')
    .post(reply);

```