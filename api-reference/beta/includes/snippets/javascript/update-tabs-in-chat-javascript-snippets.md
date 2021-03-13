---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf0ab7351a660e76295a8049e7910ae36be97421
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsTab = {
  displayName: 'My Contoso Tab - updated again'
};

await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs/794f0e4e-4d10-4bb5-9079-3a465a629eff')
    .version('beta')
    .update(teamsTab);

```