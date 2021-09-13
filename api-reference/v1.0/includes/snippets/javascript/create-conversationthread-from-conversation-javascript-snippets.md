---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1a8b3124f36068d570e35df8a4462765d323e8a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
    topic: 'Take your wellness days and rest',
    posts: [
        {
            body: {
                contentType: 'html',
                content: 'Waiting for the summer holidays.'
            }
        }
    ]
};

await client.api('/groups/{id}/conversations/{id}/threads')
    .post(conversationThread);

```