---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4829b6c39c83f9c21b2a502439141734d81ce8d7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957860"
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