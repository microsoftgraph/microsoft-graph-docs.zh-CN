---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14344b195d99e34325f60bfc8eff86030d99ddfc
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2020
ms.locfileid: "48601632"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScoreControlProfiles/{id}')
    .get();

```