---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df102db49c2fe8f9c350266455d7d2b1547b503b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105890"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistrationQuestion = {
  displayName: 'What\'s your job position?',
  isRequired: false,
  answerInputType: 'text'
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/microsoft.graph.meetingRegistration/customQuestions')
    .version('beta')
    .post(meetingRegistrationQuestion);

```