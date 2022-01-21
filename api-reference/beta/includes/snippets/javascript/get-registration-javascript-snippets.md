---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9028ac360ae3f94212843f791470e7609d60522
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102824"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let meetingRegistration = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration')
    .version('beta')
    .expand('customQuestions')
    .get();

```