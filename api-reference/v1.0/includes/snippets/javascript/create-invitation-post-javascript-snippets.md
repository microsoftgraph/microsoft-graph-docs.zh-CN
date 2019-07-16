---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ce69b87e4aa320b26580046ccb992fe5094bf6b6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738736"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const invitation = {
  invitedUserEmailAddress: "yyy@test.com",
  inviteRedirectUrl: "https://myapp.com"
};

let res = await client.api('/invitations')
    .post({invitation : invitation});

```