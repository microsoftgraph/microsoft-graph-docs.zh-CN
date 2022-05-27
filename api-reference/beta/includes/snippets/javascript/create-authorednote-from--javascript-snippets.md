---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04896349a18d2a93ee79ac0cc7b11548960eb1a9
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authoredNote = {
    content: {
        content: 'Please take a look at the files tagged with follow up',
        contentType: 'text'
    }
};

await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes')
    .version('beta')
    .post(authoredNote);

```