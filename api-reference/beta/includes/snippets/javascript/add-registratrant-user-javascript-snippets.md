---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e461361b285e842f2c7fc554d6f92c61f47bfc5d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistrantBase = {
  '@odata.type': '#microsoft.graph.meetingRegistrant',
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
    .post(meetingRegistrantBase);

```