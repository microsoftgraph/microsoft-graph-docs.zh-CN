---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce91f59ef40e1bfec60556e463c94f1084f38ccda174f15160c57f22b0527baa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162877"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const offerShiftRequest = {
  senderShiftId: 'SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29',
  senderMessage: 'Having a family emergency, could you take this shift for me?',
  recipientUserId: 'fe278b61-21ac-4872-8b41-1962bbb98e3c'
};

await client.api('/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/offershiftrequests')
    .version('beta')
    .post(offerShiftRequest);

```