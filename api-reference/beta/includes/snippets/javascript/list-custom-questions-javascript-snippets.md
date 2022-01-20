---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2726dc232bc737f7160cb4d0a3628b52fe3b3f7a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customQuestions = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/microsoft.graph.meetingRegistration/customQuestions')
    .version('beta')
    .get();

```