---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31d25291d0e1ba5c0350d223b2bbc746436e4718
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationOutcome = {
    @odata.type:"#microsoft.graph.educationFeedbackOutcome",
    feedback:{
        text:{
            content:"This is feedback for the assignment as a whole.",
            contentType:"text"
        }
    }
};

let res = await client.api('/education/me/assignments/{id}/submissions/{id}/outcomes/{id}')
    .version('beta')
    .update(educationOutcome);

```