---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e19d75429a342370c8b832ed88e61a5322f57bdd
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561715"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistrant = {
  firstName: 'Lisa',
  lastName: 'Adkins',
  email: 'lisa.adkins@contoso.com',
  customQuestionAnswers: [
    {
      questionId: 'MSM5YjlmM2Q4ZS03ZmVkLTRmN3gwMDIw94MDAyMF9hX3gwMDIwX2RldmU=',
      value: 'No'
    },
    {
      questionId: 'MSM5M2E2OWQ1Ni1jZTc4LTQDAwMjBfZGlkX3gwMDIwX3lvdV94MDAyMF8=',
      value: 'Internet'
    }
  ]
};

await client.api('/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants')
    .version('beta')
    .post(meetingRegistrant);

```