---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 667d09874e330a13e71951f9d17d1819d11bc19f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/drive/root/delta?token=2021-09-29T20%3A00%3A00Z')
    .get();

```