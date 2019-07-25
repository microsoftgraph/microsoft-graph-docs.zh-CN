---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 28782297c2e9a719f5cbc31b7f2d9f129eb6450e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
    .version('beta')
    .filter('MentionsPreview/IsMentioned eq true,')
    .select('subject,sender,receivedDateTime,mentionsPreview')
    .get();

```