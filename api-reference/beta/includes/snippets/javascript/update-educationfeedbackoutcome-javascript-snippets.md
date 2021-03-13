---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90f8dd0d4f59df3e0bfb5a1a401bdded584cb58e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationOutcome = {
    '@odata.type':'#microsoft.graph.educationFeedbackOutcome',
    feedback: {
        text: {
            content: 'This is feedback for the assignment as a whole.',
            contentType: 'text'
        }
    }
};

await client.api('/education/me/assignments/{id}/submissions/{id}/outcomes/{id}')
    .version('beta')
    .update(educationOutcome);

```