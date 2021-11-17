---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af9ed23853289008ceb7945cbe915035541f1dd79f3c99205c2bc32410c58776
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219504"
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