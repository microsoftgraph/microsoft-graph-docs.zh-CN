---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78cb3385b8e394e6aa908d73badc2d2955c84e90
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const offerShiftRequest = {
  senderShiftId: "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  senderMessage: "Having a family emergency, could you take this shift for me?",
  recipientUserId: "fe278b61-21ac-4872-8b41-1962bbb98e3c"
};

let res = await client.api('/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/offershiftrequests')
    .post(offerShiftRequest);

```