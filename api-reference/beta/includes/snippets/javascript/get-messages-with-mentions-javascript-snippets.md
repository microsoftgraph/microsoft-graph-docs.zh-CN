---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d4d7fa470deb36ae6f4b42c3b66d20c91d612b7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/me/messages')
    .version('beta')
    .filter('MentionsPreview/IsMentioned eq true')
    .select('subject,sender,receivedDateTime,mentionsPreview')
    .get();

```