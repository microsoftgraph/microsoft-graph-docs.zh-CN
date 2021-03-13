---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 859e0a4be93df9a91397a0c39076e3ca5bc1ca42
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775624"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onlineMeeting = {
  lobbyBypassSettings: {
      isDialInBypassEnabled: true
  }
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi')
    .version('beta')
    .update(onlineMeeting);

```