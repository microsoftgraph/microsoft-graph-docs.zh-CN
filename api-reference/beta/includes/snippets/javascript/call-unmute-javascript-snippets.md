---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7ceb166abe704f4ea9d4fa189eace71c050e1993
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933809"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unmuteParticipantOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/unmute')
    .version('beta')
    .post(unmuteParticipantOperation);

```