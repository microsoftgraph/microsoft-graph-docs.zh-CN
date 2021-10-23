---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 040c7b8f23ec9277400e2568112bcfb4247922b1
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558609"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistrationQuestion = {
  answerInputType: 'radioButton',
  answerOptions: [
    'Software Engineer',
    'Software Development Manager',
    'Product Manager',
    'Data scientist',
    'Other'
  ]
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/customQuestions/MSNhYjc5NWI4MC119zX3gwMDIwX3lvdXJfeDAwMjBfam8=')
    .version('beta')
    .update(meetingRegistrationQuestion);

```