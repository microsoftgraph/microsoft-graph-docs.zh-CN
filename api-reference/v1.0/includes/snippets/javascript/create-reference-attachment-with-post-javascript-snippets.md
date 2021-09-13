---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1e9431fa40216b537c50f5371641d8ebc7307f4047b54262efbbd8d2875790c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328889"
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
    .post(reply);

```