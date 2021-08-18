---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5de6e7d5f740b91cfc107d49bc8d4a6e1f7ca28d0ffaa5d96415310a60f2ee64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218558"
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

await client.api('/education/classes/{id}/assignments/{id}/submissions/{id}/outcomes/{id}')
    .version('beta')
    .update(educationOutcome);

```