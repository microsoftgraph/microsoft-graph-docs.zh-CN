---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 836b58964d9730ab2029427a41ddf0028dec8a97
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/owners/{id}/$ref')
    .version('beta')
    .delete();

```