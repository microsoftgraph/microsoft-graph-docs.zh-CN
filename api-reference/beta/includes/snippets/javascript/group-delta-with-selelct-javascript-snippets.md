---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83bba234ff937c5dabd264a766a8959aea2df93c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858754"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/delta')
    .version('beta')
    .select('displayName,description,mailNickname')
    .get();

```