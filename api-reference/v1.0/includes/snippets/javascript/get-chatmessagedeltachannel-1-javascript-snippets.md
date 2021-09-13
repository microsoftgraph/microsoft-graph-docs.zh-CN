---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65362fbad262fcd674056f42310843d290b12c07b9758b454a4523b1796527a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279204"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/delta')
    .top(2)
    .get();

```