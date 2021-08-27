---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a579ea200c5d7c7bd21602a84daaea66abd02915e7440ef0ecb5384e097a24eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904275"
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

await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages')
    .version('beta')
    .post(chatMessage);

```