---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bfc10521ef2716f2530bf44c46228a0a1fa313a
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistration = {
  subject: 'Microsoft Ignite',
  description: 'Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more.',
  startDateTime: '2021-11-02T08:00:00-08:00',
  endDateTime: '2021-11-04T04:00:00-08:00',
  allowedRegistrant: 'everyone',
  speakers: [
    {
      displayName: 'Henry Ross',
      bio: 'Chairman and Chief Executive Officer'
    },
    {
      displayName: 'Hailey Clark',
      bio: 'EVP'
    }
  ],
  customQuestions: [
    {
      displayName: 'Are you a developer?',
      answerInputType: 'radioButton',
      answerOptions: [ 'Yes', 'No' ],
      isRequired: true
    },
    {
      displayName: 'Where did you hear about us?',
      answerInputType: 'text',
      isRequired: false
    }
  ]
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration')
    .version('beta')
    .post(meetingRegistration);

```