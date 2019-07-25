---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e7206f551b1c1334b771c4ba3f522cbf11513fcf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')')
    .get();

```