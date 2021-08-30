---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96ed46bb14a87bb2b7f7359c920db2771d7f4d23afcfe88229d0f1bc070d35ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta')
    .version('beta')
    .top(2)
    .get();

```