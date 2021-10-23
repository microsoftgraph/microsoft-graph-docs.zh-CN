---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 513237a5228769b91935aabdd0e862f551a88a02
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistrant = {
  firstName: 'Frederick',
  lastName: 'Cormier',
  email: 'frederick.cormier@contoso.com',
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

await client.api('/users/16664f75-11dc-4870-bec6-38c1aaa81431/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants')
    .version('beta')
    .post(meetingRegistrant);

```