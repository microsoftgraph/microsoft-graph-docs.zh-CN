---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a0b1b8e352ab2d513d011b5df69cf131fbcbad9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118899"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistrantBase = {
  '@odata.type': '#microsoft.graph.externalMeetingRegistrant',
  id: '9d96988d-a66a-46ce-aad7-0b245615b297'
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants')
    .version('beta')
    .post(meetingRegistrantBase);

```