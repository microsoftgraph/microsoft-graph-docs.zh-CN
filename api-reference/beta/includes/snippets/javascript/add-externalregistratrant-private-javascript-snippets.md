---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77ba9f6f9a64a4ac21d6073ae32b636536571cdd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistrantBase = {
  '@odata.type': '#microsoft.graph.externalMeetingRegistrant',
  id: '30494ab7-7338-4592-bfec-a4333be2a0a6',
  tenantId: '909c6581-5130-43e9-88f3-fcb3582cde37',
  userId: 'cc515404-b55c-466e-b896-992c918ecc01'
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants')
    .version('beta')
    .post(meetingRegistrantBase);

```