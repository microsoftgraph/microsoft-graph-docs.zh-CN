---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f517a34125ee5a45d33412c01962de5e4b5b82c9
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const hideForUser = {
  user: {
    id: 'd864e79f-a516-4d0f-9fee-0eeb4d61fdc2'
  },
  tenantId: '2a690434-97d9-4eed-83a6-f5f13600199a'
};

await client.api('/chats/19:7d898072-792c-4006-bb10-5ca9f2590649_8ea0e38b-efb3-4757-924a-5f94061cf8c2@unq.gbl.spaces/hideForUser')
    .version('beta')
    .post(hideForUser);

```