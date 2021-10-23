---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9028ac360ae3f94212843f791470e7609d60522
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561491"
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