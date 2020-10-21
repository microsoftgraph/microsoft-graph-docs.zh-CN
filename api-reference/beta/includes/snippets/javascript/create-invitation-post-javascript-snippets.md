---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 503fb68653de729c8f2e35652082b8ebca1fb2d6
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const invitation = {
  invitedUserEmailAddress: "yyy@test.com",
  inviteRedirectUrl: "https://myapp.contoso.com"
};

let res = await client.api('/invitations')
    .version('beta')
    .post(invitation);

```