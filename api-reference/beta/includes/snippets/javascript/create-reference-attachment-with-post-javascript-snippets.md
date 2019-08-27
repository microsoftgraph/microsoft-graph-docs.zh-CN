---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a22397f25bb0fecc8e4e2132f6956792e96d5f00
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: "text",
      content: "I attached a reference to a file on OneDrive."
    },
    attachments: [{
      @odata.type: "#microsoft.graph.referenceAttachment", 
      name: "Personal pictures", 
      sourceUrl: "https://contoso.com/personal/mario_contoso_net/Documents/Pics", 
      providerType: "oneDriveConsumer", 
      permission: "Edit", 
      isFolder: "True"
    } ]
  }
};

let res = await client.api('/groups/1848753d-185d-4c08-a4e4-6ee40521d115/threads/AAQkADJUdfolA==/reply')
    .version('beta')
    .post(reply);

```