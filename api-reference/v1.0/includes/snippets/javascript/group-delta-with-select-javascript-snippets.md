---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3b49dd26f66fca605f2d8e4f58f845c0165c65c0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890817"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/delta')
    .select('displayName,description,mailNickname')
    .get();

```