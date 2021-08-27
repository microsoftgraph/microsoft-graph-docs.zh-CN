---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47cc1cfd0d63fa5b633b6d5b9e5d3cc7cc51de69ca241b5e080db87e335e5087
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
    subject: null,
    body: {
        contentType: 'html',
        content: '<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>'
    },
    attachments: [
        {
            id: '74d20c7f34aa4a7fb74e2b30004247c5',
            contentType: 'application/vnd.microsoft.card.thumbnail',
            contentUrl: null,
            content: '{\r\n  \"title\': \'This is an example of posting a card\",\r\n  \"subtitle\': \'<h3>This is the subtitle</h3>\",\r\n  \"text\': \'Here is some body text. <br>\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\': [\r\n    {\r\n      \'type\': \'messageBack\",\r\n      \"title\': \'Login to FakeBot\",\r\n      \"text\': \'login\",\r\n      \"displayText\': \'login\",\r\n      \"value\': \"login\"\r\n    }\r\n  ]\r\n}",
            name: null,
            thumbnailUrl: null
        }
    ]
};

await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages')
    .post(chatMessage);

```