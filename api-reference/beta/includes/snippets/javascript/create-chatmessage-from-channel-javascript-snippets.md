---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 770f0232446f0eeb84fb541601739ce17228c71b
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
    subject: null,
    body: {
        contentType: "html",
        content: "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"
    },
    attachments: [
        {
            id: "74d20c7f34aa4a7fb74e2b30004247c5",
            contentType: "application/vnd.microsoft.card.thumbnail",
            contentUrl: null,
            content: {\r\n  \"title\: \This is an example of posting a card\",\r\n  \"subtitle\: \<h3>This is the subtitle</h3>\",\r\n  \"text\: \Here is some body text. <br>\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\: [\r\n    {\r\n      \type\: \messageBack\",\r\n      \"title\: \Login to FakeBot\",\r\n      \"text\: \login\",\r\n      \"displayText\: \login\",\r\n      \"value\: \"login\"\r\n    }\r\n  ]\r\n}",
            name: null,
            thumbnailUrl: null
        }
    ]
};

let res = await client.api('/teams/{id}/channels/{id}/messages')
    .version('beta')
    .post(chatMessage);

```