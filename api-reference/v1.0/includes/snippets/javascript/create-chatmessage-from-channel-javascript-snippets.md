---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dd96ca5734f649e685596f4d5e1eeb780b15544
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
    body: {
        contentType: 'html',
        content: 'Here\'s the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>'
    },
    attachments: [
        {
            id: '153fa47d-18c9-4179-be08-9879815a9f90',
            contentType: 'reference',
            contentUrl: 'https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx',
            name: 'Budget.docx'
        }
    ]
};

await client.api('/teams/{id}/channels/{id}/messages')
    .post(chatMessage);

```