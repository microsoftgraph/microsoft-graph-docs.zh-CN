---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92d7ca35ba3b3dc4f02d83c57766cc7f5fdb4829
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
    body: {
        contentType: "html",
        content: "Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"
    },
    attachments: [
        {
            id: "153fa47d-18c9-4179-be08-9879815a9f90",
            contentType: "reference",
            contentUrl: "https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx",
            name: "Budget.docx"
        }
    ]
};

let res = await client.api('/teams/{id}/channels/{id}/messages')
    .post(chatMessage);

```