---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60f69b1fadcdbbd1490d083d94fe5bddbc9a48db
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members/{id}/$ref')
    .delete();

```